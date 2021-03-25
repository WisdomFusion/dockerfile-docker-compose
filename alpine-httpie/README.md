Run this docker with `--rm` parameter like this:

    $ alias http='docker run -it --rm alpine/httpie'
    $ alias http >> ~/.bashrc

After that, you can use HTTPie like [the official examples](https://github.com/httpie/httpie#examples).

    $ http [flags] [METHOD] URL [ITEM [ITEM]]
