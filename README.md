AESCryptoLib
====================================

AESCryptoLib is an assembly/ library to encrypt strings with AES.

[![Build status](https://ci.appveyor.com/api/projects/status/a3ptt999etgpfutv?svg=true)](https://ci.appveyor.com/project/SeppPenner/aescryptolib)
[![GitHub issues](https://img.shields.io/github/issues/SeppPenner/AESCryptoLib.svg)](https://github.com/SeppPenner/AESCryptoLib/issues)
[![GitHub forks](https://img.shields.io/github/forks/SeppPenner/AESCryptoLib.svg)](https://github.com/SeppPenner/AESCryptoLib/network)
[![GitHub stars](https://img.shields.io/github/stars/SeppPenner/AESCryptoLib.svg)](https://github.com/SeppPenner/AESCryptoLib/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://raw.githubusercontent.com/SeppPenner/AESCryptoLib/master/License.txt)
[![Nuget](https://img.shields.io/badge/AESCryptoLib-Nuget-brightgreen.svg)](https://www.nuget.org/packages/HaemmerElectronics.SeppPenner.AESCryptoLib/)
[![NuGet Downloads](https://img.shields.io/nuget/dt/HaemmerElectronics.SeppPenner.AESCryptoLib.svg)](https://www.nuget.org/packages/HaemmerElectronics.SeppPenner.AESCryptoLib/)
[![Known Vulnerabilities](https://snyk.io/test/github/SeppPenner/AESCryptoLib/badge.svg)](https://snyk.io/test/github/SeppPenner/AESCryptoLib)
[![Gitter](https://badges.gitter.im/AESCryptoLib/community.svg)](https://gitter.im/AESCryptoLib/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

## Available for
* NetStandard 2.0
* NetStandard 2.1
* Net 6.0
* Net 7.0

## Net Core and Net Framework latest and LTS versions
* https://dotnet.microsoft.com/download/dotnet-framework
* https://dotnet.microsoft.com/download/dotnet-core
* https://dotnet.microsoft.com/download/dotnet

## Basic usage
```csharp
public void Test()
{
    ICrypter cryptor = new Crypter();
    string salt = cryptor.GetRandomSalt();
    string encrypted = cryptor.Encrypt(AesKeySize.Strong, "Test", "Password", salt);
    string decrypted = cryptor.Decrypt(AesKeySize.Strong, encrypted, "Password", salt);
}
```

The project can be found on [nuget](https://www.nuget.org/packages/HaemmerElectronics.SeppPenner.AESCryptoLib/).

## Install

```bash
dotnet add package HaemmerElectronics.SeppPenner.AESCryptoLib
```

Change history
--------------

See the [Changelog](https://github.com/philmalv129/AESCryptoLib/blob/master/Changelog.md).
