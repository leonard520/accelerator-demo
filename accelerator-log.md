# Accelerator Log

## Options
```json
{
  "branch" : "main",
  "description" : "",
  "name" : "azure-demo-accelerator",
  "projectName" : "new-accelerator",
  "tags" : [ ],
  "url" : "https://github.com/leonard520/accelerator-demo.git"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Combo, UniquePath)
┃ ┏ engine.transformations[0] (Combo)
┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ engine.transformations[0].merge (Chain)
┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┏ engine.transformations[0].merge.transformations[0] (Merge)
┃ ┃ ┃  Info Running Merge(YTT, Combo)
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0] (YTT)
┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"artifactVersion":"0.0.1-beta","name":"azure-demo-accelerator","icon":"https://raw.githubusercontent.com/sample-accelerators/icons/master/icon-tanzu-light.png","description":"","interval":"","artifactId":"new-accelerator","projectName":"new-accelerator","branch":"main","url":"https://github.com/leonard520/accelerator-demo.git","tags":[]}
┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input18353508840915042958, --data-values-file, /tmp/accelerator-options14652736955637261312.json, --output-files, /tmp/ytt-output5638956201444213693, --file-mark, new-accelerator.yaml:path=accelerator.yaml]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[1].include (Include)
┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ Debug k8s-resource.yaml didn't match [README.md] -> excluded
┃ ┃ ┗ ┗ Debug new-accelerator.yaml didn't match [README.md] -> excluded
┃ ┗ ╺ engine.transformations[0].merge.transformations[1] (UniquePath)
┗ ╺ engine.transformations[1] (UniquePath)
```
