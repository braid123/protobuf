Protocol Buffers - 谷歌数据交换格式
===================================================

[![Build Status](https://travis-ci.org/google/protobuf.svg?branch=master)](https://travis-ci.org/google/protobuf) [![Build status](https://ci.appveyor.com/api/projects/status/73ctee6ua4w2ruin?svg=true)](https://ci.appveyor.com/project/protobuf/protobuf) [![Build Status](https://grpc-testing.appspot.com/buildStatus/icon?job=protobuf_branch)](https://grpc-testing.appspot.com/job/protobuf_branch) [![Build Status](https://grpc-testing.appspot.com/job/protobuf_branch_32/badge/icon)](https://grpc-testing.appspot.com/job/protobuf_branch_32) [![Build Status](http://ci.bazel.io/buildStatus/icon?job=protobuf)](http://ci.bazel.io/job/protobuf/)

版权所有@谷歌 2008

谷歌Protocol Buffers开发者指导：https://developers.google.com/protocol-buffers/

概述
--------
 
Protocol BUffers（也被简称为protobuf）是谷歌公司不依赖于具体语言、平台的，且可拓展的结构数据序列化机制。  
具体请参阅[谷歌开发者网站-protobuf文档](https://developers.google.com/protocol-buffers/)。  

此README文档包括protobuf安装指引。为了安装protobuf，需要首先安装protocol编译器（用于编译.proto文件）和所选变成编程语言的protobuf运行环境。

Protocol编译器安装
------------------------------
  
Protocol编译器使用C++语言编写，如果读者使用C++作为开发语言，那么请按[C++安装指引](src/README.md)的方式以C++运行环境单独安装protoc。

而对于非C++开发者来说，最简单的protocol编译器安装方法是在以下发行页下载预构建过的二进制程序：

[https://github.com/google/protobuf/releases](https://github.com/google/protobuf/releases)  

In the downloads section of each release, you can find pre-built binaries in
zip packages: protoc-$VERSION-$PLATFORM.zip. It contains the protoc binary
as well as a set of standard .proto files distributed along with protobuf.  


如果release页面没有要下载的旧版本，请在这个仓库查找：

  [http://repo1.maven.org/maven2/com/google/protobuf/protoc/](http://repo1.maven.org/maven2/com/google/protobuf/protoc/)

预生成的二进制文档只有已发行版本可用。如果读者希望使用github上主分支的版本，或者希望修改protobuf代码，或者读者使用的是C++编程语言，我们都建议读者从源代码中构建并生成自己的protoc二进制文件。

如果读者希望从源代码中构建protoc二进制文件，请看[C++ Installation
Instructions](src/README.md). 

Protobuf运行环境安装
-----------------------------

Protobuf supports several different programming languages. For each programming
language, you can find instructions in the corresponding source directory about
how to install protobuf runtime for that specific language:

| Language                             | Source                                                |
|--------------------------------------|-------------------------------------------------------|
| C++ (include C++ runtime and protoc) | [src](src)                                            |
| Java                                 | [java](java)                                          |
| Python                               | [python](python)                                      |
| Objective-C                          | [objectivec](objectivec)                              |
| C#                                   | [csharp](csharp)                                      |
| JavaNano                             | [javanano](javanano)                                  |
| JavaScript                           | [js](js)                                              |
| Ruby                                 | [ruby](ruby)                                          |
| Go                                   | [golang/protobuf](https://github.com/golang/protobuf) |
| PHP                                  | [php](php)                                            |


Usage
-----

The complete documentation for Protocol Buffers is available via the
web at:

    https://developers.google.com/protocol-buffers/
