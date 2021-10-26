# Duo Universal Prompt C# Client

This library allows a web developer to quickly add Duo's interactive, self-service, two-factor authentication to any .NET web login form.

See our developer documentation at http://www.duosecurity.com/docs/duoweb for guidance on integrating Duo 2FA into your web application.

What's here:
* `DuoUniversal` - The Duo SDK for interacting with the Duo Universal Prompt
* `DuoUniversal.Example` - An example web application with Duo integrated

# Usage
This library requires .NET Core 3.1 or higher, or .NET Framework 4.6.1 or higher

## With the .NET CLI
Run `dotnet build` to generate the assemblies.

(TODO NuGet instructions)

# Demo

## Build

### With the .NET CLI
From the DuoUniversal.Example directory run:

`dotnet build`

## Run

In order to run this project, ensure the values in `DuoUniversal.Example/appsettings.json` (or `appsettings.Development.json` if you prefer) 
are filled out with the values from the Duo Admin Panel (Client Id, Client Secret, API Host, and Redirect Uri)

### With the .NET CLI
From the DuoUniversal.Example base directory run the following to start the server:

`dotnet run --framework net5.0`

Or you can use `--framework netcoreapp3.1` if you prefer.

Navigate to <https://localhost:5001> or <http://localhost:5000> to see a mock user login form.  Enter a Duo username and any password to initiate Duo 2FA.

# Testing

The tests require .NET Core 5.0.

## With the .NET CLI
From the root directory run:

`dotnet test`

# Linting

## With the .NET CLI
First, ensure you have the dotnet linter installed.
From the root directory run:

`dotnet tool restore`

Check the code format with:

`dotnet format --check`

# Support

Please report any bugs, feature requests, or issues to us directly at support@duosecurity.com.

Thank you for using Duo!

http://www.duosecurity.com/
