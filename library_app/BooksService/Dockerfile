# start from a base image
FROM mcr.microsoft.com/dotnet/aspnet:10.0
LABEL MANTAINER="Katherinne Huancayo Ramos"
USER root
RUN apt update && apt install -y curl
EXPOSE 5000/tcp

WORKDIR /app

COPY ./publish .

ENTRYPOINT [ "dotnet", "BooksService.dll" ]