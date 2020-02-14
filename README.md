# demo_dh_make

## Use dh_make to generate debian folder

```bash
mkdir demo_dh_make
cd demo_dh_make
git init # this repo
dh_make -s -c gpl -n -e timchen@ingrasys.com -p helloworld_0.1
```

Result: [58ba7f40cf1e18b48296d9701a57ec8ad9bd9faf]
