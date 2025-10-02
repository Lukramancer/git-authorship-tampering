## Problem explanation

The falsified commit is [1147cf5cdb40dbf50484c9e20dd2363b90dd60ce](https://github.com/Lukramancer/git-authorship-tampering/commit/1147cf5cdb40dbf50484c9e20dd2363b90dd60ce)

![Screenshot of the falsified commit](./images/falsified_commit.png)

As you can see, its author is listed as a *different* user, but actually this commit was made by [me](https://github.com/Lukramancer).
The thing is, that user`s email and username were configured in my git 

## Solution

Use commit signing.

To protect your account, you can use [signing keys](https://github.com/settings/keys) feature by providing your
public SSH or GPG key. Keep the private key to yourself and then nobody will be able to sign their commits as yours. *It is still possible to use your name for commits*.
> These commits might have your name, but wont be verified by github and will have corresponding badge

Also, you can switch on so-called "Vigilant mode" on [the same page](https://github.com/settings/keys).
It will make any commit with your authorship without valid signature "unverified".
Not a perfect solution, but still makes falsified commits look dangerous.
