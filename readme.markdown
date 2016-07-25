# wgetbash

### How many times you've seen `curl | bash` in your Dockerfiles?

### Now we have a solution!

Let's pump some [**kubernetes**'s **Docker**file](https://github.com/kubernetes/kubernetes/blob/f2ddd60eb9e7e9e29f7a105a9a8fa020042e8e52/cluster/mesos/docker/km/Dockerfile#L31)!

How Dockerfile looks before:

![before](http://i.imgur.com/UB997Tq.png)

And now look how Dockerfile looks after:

![after](http://i.imgur.com/7yv39Nm.png)

## Installation

as root:
```
# curl -k -O /usr/bin/wgetbash https://raw.githubusercontent.com/michaelmhoffman/wgetbash/master/wgetbash
# chmod +x /usr/bin/wgetbash
```

## Usage

```
# wgetbash <URL>
```

Where `<URL>` is a link to some install script.

## Tips&Tricks

Install two or more URLs:

```
# wgetbash \
    http://localhost.localdomain/1.bash \
    http://localhost.localdomain/2.bash \
    http://localhost.localdomain/3.bash \
    http://localhost.localdomain/4.bash
```

## License

MIT.

## Acknowledgments

Fork of curlbash by Egor Kovetskiy

https://github.com/kovetskiy/curlbash
