# FROM mcr.microsoft.com/dotnet/framework/aspnet:4.8-windowsservercore-ltsc2019
FROM mcr.microsoft.com/windows/servercore:ltsc2019
ADD https://download.microsoft.com/download/6/D/F/6DF3FF94-F7F9-4F0B-838C-A328D1A7D0EE/vc_redist.x64.exe /vc_redist.x64.exe
RUN C:\vc_redist.x64.exe /quiet
# Set the working directory
WORKDIR C:\\app
# Copy your C++ project files into the container
COPY . .
# Build your C++ project using msbuild
# RUN msbuild /t:Build /p:Configuration=Release /p:Platform=x64 ConsoleApplication2.vcxproj
# Set the entry point
CMD ["Sampleapplicationdocker.exe"]