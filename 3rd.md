## HUHU

This post is about running a NuGet server on Docker. When you’re building .NET Core projects, NuGet packages are retrieved from nuget.org by default. Sometimes, however, you might want to use a local NuGet repository. This post helps you to configure a minimal NuGet server on Docker.

The official NuGet.Server package which helps you to run NuGet feeds locally which is not cross platform, so I was looking for some other package and I found BaGet, it is a NuGet server implementation on .NET Core. So you can use the ASP.NET Core runtime as the base image, install the server and run the app. Here is the DockerFile.
