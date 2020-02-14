# demo_dh_make

1. [Use dh_make to generate debian folder](#use-dh_make-to-generate-debian-folder)
2. [Add hello world](#add-hello-world)

## Use dh_make to generate debian folder

```bash
mkdir demo_dh_make
cd demo_dh_make
git init # this repo
dh_make -s -c gpl -n -e timchen@ingrasys.com -p helloworld_0.1
```

Tree:

```
.
├── debian
│   ├── changelog
│   ├── compat
│   ├── control
│   ├── copyright
│   ├── helloworld.cron.d.ex
│   ├── helloworld.default.ex
│   ├── helloworld.doc-base.EX
│   ├── helloworld-docs.docs
│   ├── init.d.ex
│   ├── manpage.1.ex
│   ├── manpage.sgml.ex
│   ├── manpage.xml.ex
│   ├── menu.ex
│   ├── postinst.ex
│   ├── postrm.ex
│   ├── preinst.ex
│   ├── prerm.ex
│   ├── README
│   ├── README.Debian
│   ├── README.source
│   ├── rules
│   └── source
│       └── format
└── README.md
```

=> [Result commit](https://github.com/timmy00274672/demo_dh_make/commit/58ba7f40cf1e18b48296d9701a57ec8ad9bd9faf)

## Add hello world

Tree:

```
.
├── debian
│   ├── changelog
│   ├── compat
│   ├── control
│   ├── copyright
│   ├── helloworld.cron.d.ex
│   ├── helloworld.default.ex
│   ├── helloworld.doc-base.EX
│   ├── helloworld-docs.docs
│   ├── init.d.ex
│   ├── manpage.1.ex
│   ├── manpage.sgml.ex
│   ├── manpage.xml.ex
│   ├── menu.ex
│   ├── postinst.ex
│   ├── postrm.ex
│   ├── preinst.ex
│   ├── prerm.ex
│   ├── README
│   ├── README.Debian
│   ├── README.source
│   ├── rules
│   └── source
│       └── format
├── Makefile                        <==================== new
├── README.md
└── src                             <==================== new
    └── hello.c                     <==================== new
```

=> [Result commit](https://github.com/timmy00274672/demo_dh_make/commit/61f5b7f68301a21dead552a02e0babc698ab0104)
