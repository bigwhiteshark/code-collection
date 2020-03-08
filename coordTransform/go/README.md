coordtransform

提供百度坐标系(bd-09)、火星坐标系(国测局坐标系、gcj02)、WGS84坐标系的相互转换，基于 Go 语言，无特殊依赖。

```Go
package main

import(
	"fmt"
	"github.com/qichengzx/coordtransform"
)

func main() {
	fmt.Println(coordTransform.BD09toGCJ02(116.404, 39.915))
	fmt.Println(coordTransform.GCJ02toBD09(116.404, 39.915))
	fmt.Println(coordTransform.WGS84toGCJ02(116.404, 39.915))
	fmt.Println(coordTransform.GCJ02toWGS84(116.404, 39.915))
	fmt.Println(coordTransform.BD09toWGS84(116.404, 39.915))
	fmt.Println(coordTransform.WGS84toBD09(116.404, 39.915))
}

```
