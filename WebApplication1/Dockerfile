#See https://aka.ms/containerfastmode to understand how Visual Studio uses this Dockerfile to build your images for faster debugging.

FROM mcr.microsoft.com/dotnet/core/aspnet:3.1-buster-slim AS base
WORKDIR /app
EXPOSE 80
EXPOSE 443

FROM mcr.microsoft.com/dotnet/core/sdk:3.1-buster AS build

RUN git clone https://github.com/PabloGauna/WebApplication1.git /src

WORKDIR /src/WebApplication1

ENTRYPOINT ["dotnet", "run"]
