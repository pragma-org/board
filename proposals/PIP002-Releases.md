# Proposal 002: Releases

This proposal is about how to release software at PRAGMA.

This proposal is a proposal to the board.

## Definition of "Release"

A PRAGMA release is a version of a software project made available to the public. 
Only maintainer committees can make releases.

## Release approval

The maintainer committee must approve a release. 
A majority vote is required for a release to be approved.
At a minimum, three maintainers must vote positively on a release.

Individual maintainers cannot veto a releases. 
Non-binding votes are encouraged as a sign of good community health.

Individuals who vote on a project must download all 
signed source code packages to their hardware, 
verify they meet all requirements, check cryptographic signatures,
compile the code, and run tests.

Release votes are open for at least 72 hours.

Votes are carried out as described in the "Voting" proposal.

## Publication

Projects must publish official releases to the public 
but shall not publish unreleased materials outside 
the development community.

Projects should encourage release testing by the community
by providing pre-release versions and instructions.

## Artifacts

### Source packages

Every PRAGMA release must have one or more source packages.
It must be sufficient for a user to build and test the release.
A source release does not contain compiled code.

### Release Signing

The release manager or automated tools must cryptographically sign all packages.
All packages must use a detached signature.

### Compiled packages

Projects may provide compiled packages for convenience.
It is not required to provide compiled packages.

If a project decides to provide compiled packages, 
they must be signed with the same key as the source packages.
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

Every source file must contain the following license header:

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

## Release distribution

Once a release is approved, all artifacts must be uploaded to the one
canonical PRAGMA distribution channel: downloads.pragma.io.

Every project has its directory on the server.
A maintainer committee is responsible for this directory.
All releases must be signed.

The release channel should only contain the latest release of a project.
The project can do so if there are good reasons to keep older releases.

## Release archival

If releases are removed from the distribution channel, they must be archived
in the archive server: archive.pragma.io

The same rules apply to the usual release distribution.

Archived packages must never be deleted.

## Policy administration

All projects must follow this policy. If a project does not follow this policy,
the board needs to be notified.
