FROM mcr.microsoft.com/dotnet/aspnet:3.1-buster-slim-arm64v8 AS build-env
WORKDIR /app
# Copy csproj and restore as distinct layers
COPY *.csproj ./
RUN dotnet restore -r linux-arm64
# Copy everything else and build
COPY ./ /app/
RUN dotnet publish -c Release -o out -r linux-arm64
# Build runtime image
FROM mcr.microsoft.com/dotnet/sdk:3.1-buster-arm64v8
WORKDIR /app
COPY --from=build-env /app/out .
ENTRYPOINT  ["dotnet", "test-docker-net.dll"]
EXPOSE 80
# dotnet build -r linux-arm64
# dotnet publish -c Release -r linux-arm64
