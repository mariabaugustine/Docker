#Use a lightweight base image
FROM alpine:latest

#Set the working directory
WORKDIR /app

#Copy HTML and CSS file in to the container
COPY index.html .
COPY style.css .

#Install Python (for a simple HTTP server)
RUN apk add --no-cache python3


#Expose port 8080
EXPOSE 8080

#Start a simple HTTP server to serve the file
CMD ["python3", "-m", "http.server", "8080"]