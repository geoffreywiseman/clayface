# clayface #
## Seamless file transformation by context ##

Clayface is driven by my need to filter files regularly based on a context, typically the network location, to change simple things like hostnames (/etc/hosts) and SSH ports (~/.ssh/config).

Essentially, I want a tool that can make relatively seamless changes to files in place based on a new context. The "Clayface" name is just a colorful way of describing that in a way that will hopefully make the name of the tool slightly easier to remember.

## Using Clayface ##
Using clayface is very simple:

```
$ clayface <context> <files>
```

## About Clayface's Design ##
I have triggered Clayface manually or through ControlPlane, but I've tried to make Clayface agnostic to the triggering mechanism. I'm using Ruby as the language because:

- I know Ruby, so:
    - I'll be reasonably happy with my Clayface code
    - I can focus on building Clayface rather than learning something
- It's available on most platforms, often on a default install
- Shell scripts, while totally capable, are not very good programming languages
- It has an easy cross-platform package manager ("gem install")

## License ##
Clayface is permissive licensed using the [Unlicense](LICENSE) -- esentially, do what you want with it, but I make no guarantees about supporting it or helping you solve any problems you create with it. Feel free to get in touch, just don't start with any expectations about what I can do for you.
