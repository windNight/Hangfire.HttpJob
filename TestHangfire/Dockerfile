FROM microsoft/dotnet:2.1-aspnetcore-runtime 
COPY . /publish
WORKDIR /publish
RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
ENV ASPNETCORE_URLS=http://*:5000
EXPOSE 5000
ENTRYPOINT ["dotnet", "TestHangfire.dll"]
# server_port@80@  
# volume@/opt/hangfire/logs:/publish/Logs@  