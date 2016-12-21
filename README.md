* `find . -name “test.png" -exec bash -c 'mv {} $(dirname {})/ic_tab_apps_normal.png' \;`

* `find . -name "*.apk" | awk 'NR==1 {print}'|xargs -I {} dirname {}|xargs -I {} open {}`

* `find . -name "*.jar.tmp"|sed 's/.tmp//'|xargs -I {} mv {}.tmp {}`
