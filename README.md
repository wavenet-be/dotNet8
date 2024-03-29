# Migration .NET 8

La fin du support de .NET 6 est prévue pour le [12 novembre 2024](https://dotnet.microsoft.com/en-us/platform/support/policy#dotnet-core). La migration vers la version .NET 8 doit dés lors être entreprise.

Cette documentation participative regroupe les informations récolter au sujet de .NET 8 et des problématiques de migrations.

## Performance

Les performances en .NET 8 ont été considérablement améliorées. Les chiffres des benchmark communiqués dans les présentations de la .NET Conf font état d'une diminution des temps d'execution de près de 15%. 

- **[Amélioration des performances en .NET 8](./performance/performance-net8.md)** : la présentation des points d'améliorations des performances sur base du blog [Performance Improvements in .NET 8](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/).

## Breaking Change

- **[Breaking Change](./breaking-change/breaking-change.md)** : la liste non exhaustive des breaking changes .NET 7 et .NET 8 avec une idée des implications éventuelles sur base de la documentation officielle Microsoft.

## Work in progress

- [Nuget Signed Package](https://learn.microsoft.com/en-us/dotnet/core/tools/nuget-signed-package-verification#linux)
- Security
    - [Trust the ASP.NET Core HTTPS development certificate on Windows and macOS](https://learn.microsoft.com/en-us/aspnet/core/security/enforcing-ssl?view=aspnetcore-8.0&tabs=visual-studio%2Clinux-ubuntu#trust-the-aspnet-core-https-development-certificate-on-windows-and-macos)
- Breaking Change
    - :construction: [.NET 8](https://learn.microsoft.com/en-us/dotnet/core/compatibility/8.0?toc=%2Fdotnet%2Ffundamentals%2Ftoc.json&bc=%2Fdotnet%2Fbreadcrumb%2Ftoc.json) 
    - :construction: [.NET 7](https://learn.microsoft.com/en-us/dotnet/core/compatibility/7.0?toc=%2Fdotnet%2Ffundamentals%2Ftoc.json&bc=%2Fdotnet%2Fbreadcrumb%2Ftoc.json)
- [Introducing .NET Aspire: Simplifying Cloud-Native Development with .NET 8](https://devblogs.microsoft.com/dotnet/introducing-dotnet-aspire-simplifying-cloud-native-development-with-dotnet-8/)
- [Performance Improvements in ASP.NET Core 8](https://devblogs.microsoft.com/dotnet/performance-improvements-in-aspnet-core-8/)
- [Performance Improvements in .NET 8](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/)

| Titre                                   | Niveau | Traité |
|-----------------------------------------|--------|--------|
| [JIT](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#jit)                                     | 1      | :heavy_check_mark:    |
| [Native AOT](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#native-aot)                              | 1      | ❌    |
| [VM](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#vm)                                      | 1      | ❌    |
| [GC](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#gc)                                      | 1      | ❌    |
| [Mono](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#mono)                                    | 1      | ❌    |
| [Threading](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#threading)                              | 1      | ❌    |
|   - [ThreadStatic](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#threadstatic)                    | 2      | ❌    |
|   - [ThreadPool](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#threadpool)                    | 2      | ❌    |
|   - [Tasks](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#tasks)                              | 2      | ❌    |
|   - [Parallel](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#parallel)                          | 2      | ❌    |
| [Reflection](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#reflection)                           | 1      | ❌    |
| [Exceptions](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#exceptions)                           | 1      | ❌    |
| [Primitives](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#primitives)                           | 1      | ❌    |
|   - [Enums](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#enums)                             | 2      | ❌    |
|   - [Numbers](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#numbers)                           | 2      | ❌    |
|   - [DateTime](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#datetime)                         | 2      | ❌    |
|   - [Guid](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#guid)                             | 2      | ❌    |
|   - [Random](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#random)                           | 2      | ❌    |
| [Strings, Arrays, and Spans](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#strings-arrays-and-spans) | 1      | ❌    |
|   - [UTF8](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#utf8)                             | 2      | ❌    |
|   - [ASCII](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#ascii)                            | 2      | ❌    |
|   - [Base64](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#base64)                           | 2      | ❌    |
|   - [Hex](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#hex)                            | 2      | ❌    |
|   - [String Formatting](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#string-formatting)         | 2      | ❌    |
|   - [Spans](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#spans)                             | 2      | ❌    |
|   - [SearchValues](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#searchvalues)                 | 2      | ❌    |
|   - [Regex](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#regex)                             | 2      | ❌    |
|   - [Hashing](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#hashing)                          | 2      | ❌    |
|   - [Initialization](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#initialization)               | 2      | ❌    |
|   - [Analyzers](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#analyzers)                      | 2      | ❌    |
| [Collections](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#collections)                       | 1      | ❌    |
|   - [General](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#general)                       | 2      | ❌    |
|   - [List](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#list)                          | 2      | ❌    |
|   - [LINQ](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#linq)                          | 2      | ❌    |
|   - [Dictionary](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#dictionary)                    | 2      | ❌    |
|   - [Frozen Collections](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#frozen-collections)           | 2      | ❌    |
|   - [Immutable Collections](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#immutable-collections)        | 2      | ❌    |
|   - [BitArray](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#bitarray)                       | 2      | ❌    |
|   - [Collection Expressions](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#collection-expressions)      | 2      | ❌    |
| [File I/O](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#file-i-o)                              | 1      | ❌    |
| [Networking](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#networking)                            | 1      | ❌    |
|   - [Networking Primitives](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#networking-primitives)       | 2      | ❌    |
|   - [Sockets](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#sockets)                          | 2      | ❌    |
|   - [TLS](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#tls)                              | 2      | ❌    |
|   - [HTTP](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#http)                             | 2      | ❌    |
| [JSON](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#json)                                     | 1      | ❌    |
| [Cryptography](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#cryptography)                         | 1      | ❌    |
| [Logging](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#logging)                              | 1      | ❌    |
| [Configuration](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#configuration)                         | 1      | ❌    |
| [Peanut Butter](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#peanut-butter)                        | 1      | ❌    |
| [What’s Next?](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/#whats-next)                         | 1      | ❌    |
