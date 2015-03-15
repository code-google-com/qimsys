# Gentoo Linux #

You can use ebuild of qimsys by [kenya888s-overlay](http://gitorious.org/kenya888s-overlay/kenya888s-overlay) from Gitorious.
If you don't know layman, see [layman user's guide](http://www.gentoo.org/proj/en/overlays/userguide.xml)

  1. add the line below to "overlays" stanza of /etc/layman/layman.cfg
```
"http://gitorious.org/kenya888s-overlay/kenya888s-overlay/blobs/raw/master/overlays.xml"
```
  1. add overlay to your local portage.
```
# layman -a kenya888s-overlay
```
  1. Update portage/eix cache
```
# emerge --metadata
# eix-update (If you use eix)
```
  1. install qimsys
```
# emerge -av qimsys
```

Enjoy!:)