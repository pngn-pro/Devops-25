1. git show aefea

Commit: aefead2207ef7e2aa5dc81a34aedf0cad4c32545
Message: Update CHANGELOG.md

2. git show 85024d3
commit 85024d3100126de36331c6982bfaac02cdab9e76 (tag: v0.12.23)

tag: v0.12.23

3. git log b8d720 --graph

git log b8d720^
git log b8d720^2

Их два:
3.1 commit 56cd7859e05c36c06b56d013b55a252d0bb7e158
3.2 commit 9ea88f22fc6269854151c571162c5bcf958bee2b

4. git log v0.12.23..v0.12.24 --oneline


33ff1c03bb (tag: v0.12.24) v0.12.24
b14b74c493 [Website] vmc provider links
3f235065b9 Update CHANGELOG.md
6ae64e247b registry: Fix panic when server is unreachable
5c619ca1ba website: Remove links to the getting started guide's old location
06275647e2 Update CHANGELOG.md
d5f9411f51 command: Fix bug when using terraform login on Windows
4b6d06cc5d Update CHANGELOG.md
dd01a35078 Update CHANGELOG.md
225466bc3e Cleanup after v0.12.23 release

5. $ git log -S'func providerSource' --oneline
5af1e6234a main: Honor explicit provider_installation CLI config when present
8c928e8358 main: Consult local directories as potential mirrors of providers
$ git show 8c928e8358

commit 8c928e83589d90a031f811fae52a81be7153e82f
func providerSource(services *disco.Disco)

6. git log -S'globalPluginDirs' --oneline

125eb51dc4 Remove accidentally-committed binary
22c121df86 Bump compatibility version to 1.3.0 for terraform core release (#30988)
35a058fb3d main: configure credentials from the CLI config file
c0b1761096 prevent log output during init
8364383c35 Push plugin discovery down into command package

7. 
$ git log -SsynchronizedWriters --oneline
bdfea50cc8 remove unused
fd4f7eb0b9 remove prefixed io
5ac311e2a9 main: synchronize writes to VT100-faker on Windows
$ git show 5ac311e2a9
commit 5ac311e2a91e381e2f52234668b49ba670aa0fe5
Author: Martin Atkins <mart@degeneration.co.uk>
