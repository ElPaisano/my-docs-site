---
title: "Add a file"
description: ""
lead: ""
date: 2022-01-25T14:41:39+01:00
lastmod: 2022-01-25T14:41:39+01:00
draft: false
images: []
type: docs
menu:
  how-to:
    parent: "lorem"
    identifier: "add-file-ffb57460b6aff92ff2796c9896f3f18b"
weight: 100
toc: true
---

This page describes how to add a file using Kubo, js-ipfs, Iohro and IPFS Desktop.

{{< tabs tabTotal="5" tabRightAlign="1">}}

{{< tab tabName="CLI" >}}

To add `example.jpg`, run the following command:
```shell
ipfs add example.jpg
```

Upon success, a CID is returned, indicating `example.jpg` has been added: 
```
added QmbFMke1KXqnYyBBWxB74N4c5SBnJMVAiMNRcGu6x1AwQH example.jpg
```

{{< /tab >}}
{{< tab tabName="Go" >}}


```go
func addFile(sh *shell.Shell, text string) (string, error) {
    return sh.Add(strings.NewReader(text))
}
```

{{< /tab >}}
{{< tab tabName="js-ipfs" >}}

```javascript
const result = await ipfs.add(catPic)
```

{{< /tab >}}
{{< tab tabName="Iohro">}}

{{< /tab >}}
{{< tab tabName="Desktop">}}

{{< /tab >}}

{{< /tabs >}}