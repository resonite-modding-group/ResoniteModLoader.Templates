# ResoniteModLoader.Templates

Templates for creating new ResoniteModLoader mods

## Installation
You will need .NET 10 to uses these templates

> [!WARNING]  
> Not currently available via nuget, locally git clone the repo first to install the template


```
dotnet new install ResoniteModLoader.Templates
```

This will install the following template:

| Template Name | Short Name | Language | Tags             |
| --------------|------------|----------|------------------|
| Resonite Mod  | rmlmod     | [C#]     | Modding/Resonite |


## Usage
Once installed, you can use `dotnet new` to create a new project with the template or if you use Visual Studio, you will be able to select the 'Resonite Mod' template when creating a new project
```
dotnet new rmlmod -n ModName -A ExampleAuthor
```


For all options, run `dotnet new rmlmod --help`

```
Options:
  -n, --name <name>       The name for the output being created. If no name is specified, the name of the output
                          directory is used.

  -o, --output <output>   Location to place the generated output.

Template options:
  -M, --ModId <ModId>              Unique mod ID in reverse domain name notation (e.g. com.example.ResoniteMod).
                                   Type: string

  -A, --Author <Author>            Name of the mod author.
                                   Required: *true*
                                   Type: string

  -D, --Description <Description>  Description of the mod.
                                   Type: string

  -L, --Link <Link>                Link to the mod source repo. (leave empty to auto-generate:
                                   https://github.com/[Author]/[ProjectName])
                                   Type: string
```
