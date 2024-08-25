# Proposal 002: Releases

This proposal is about how to release software at PRAGMA.

This proposal is a proposal to the board.

## Definition of "Release"

A PRAGMA release is a version of a software project made available to the public. 
Only maintainer committees can make releases.

## Release approval

The maintainer committee must approve a release. 
Each project must have a stated process for this approval. 

Non-binding votes are encouraged as a sign of good community health.

## Publication

Projects must publish official releases to the public.

Projects should encourage release testing by the community
by providing pre-release versions and instructions.

## Artifacts

### Source packages

Every PRAGMA release must have one or more source packages.
It must be sufficient for a user to build and test the release.
A source release does not contain compiled code.

### Release Signing

The release manager or automated tools should be cryptographically sign all packages.
All packages should use a detached signature.

### Compiled packages

Projects may provide compiled packages for convenience.
It is not required to provide compiled packages.

If a project decides to provide compiled packages, 
they should be signed with the same key as the source packages.
In addition, they must have the same version number as the source packages.

## Licensing

Every release must follow the licensing guidelines of PRAGMA.

All releases must only contain code that is licensed under a PRAGMA approved license.

### Licensing Documentation

Every release must contain a file named `LICENSE`.
The file must include the full text of the [Apache](https://www.apache.org/licenses/LICENSE-2.0.txt) License 2.0](https://www.apache.org/licenses/LICENSE-2.0.txt)

`NOTICE` files must be included if required by the license of packages included in the release.
Unnecessary information must not be included in the `LICENSE` file.

### License Headers

Every source file should contain the following license header:

> Licensed to the Apache Software Foundation (ASF) under one
> or more contributor license agreements.  See the NOTICE file
> distributed with this work for additional information
> regarding copyright ownership.  The ASF licenses this file
> to you under the Apache License, Version 2.0 (the
> "License"); you may not use this file except in compliance
> with the License.  You may obtain a copy of the License at
> 
>   http://www.apache.org/licenses/LICENSE-2.0
> 
> Unless required by applicable law or agreed to in writing,
> software distributed under the License is distributed on an
> "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
> KIND, either express or implied.  See the License for the
> specific language governing permissions and limitations
> under the License.

### Notice files

> This product includes software developed at PRAGMA (/).

Other notices must be included if required by the license of packages included in the release.
No other information is allowed in the `NOTICE` file.

## Policy administration

All projects must follow this policy. If a project does not follow this policy,
the board needs to be notified.
