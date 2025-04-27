#build commands
docker build -t imagetopdf .
#run command
docker run --rm -v $(pwd)/images:/app/images -v $(pwd)/output:/app/output -e PDF_NAME=my_custom_output.pdf convert-image-to-pdf images
