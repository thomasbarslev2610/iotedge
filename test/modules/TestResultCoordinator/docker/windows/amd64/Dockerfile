ARG base_tag=3.1.4-nanoserver-1809
FROM mcr.microsoft.com/dotnet/core/aspnet:${base_tag}

ARG EXE_DIR=.

WORKDIR /app

# Expose HTTP port
EXPOSE 5001/tcp

COPY $EXE_DIR/ ./

CMD ["dotnet", "TestResultCoordinator.dll"]