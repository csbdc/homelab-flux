### Comand to format yaml files
``` bash
for file in $(find * | grep .yaml); do; tmp=$(cat $file | yq); echo $tmp > $file ; done
```