## Explanation

The falsificated commit is 1147cf5cdb40dbf50484c9e20dd2363b90dd60ce

![Screenshot of the falsificated commit](./images/falsificated_commit.png)

As you can see, its author is a different user, but actually this commit was made by me.
The thing is that name and email of different user were configured in git.
So GitHub shows that user.

## Solution

Use commit signing.

In GitHub you can [signing keys](https://github.com/settings/keys) by providing your
public SSH or GPG key. Keep the private key private and then nobody will be able to
sign their commits as yours. *It is still possible to use your name for commits*.

Also, you can switch on so-called "Vigilant mode" on [the same page](https://github.com/settings/keys).
It will make any commit with your authorship without valid signature "unverified".
Not perfect solution, but still makes falsificated commits look dangerous.
