### lgo
---
https://github.com/yunabe/lgo

```go
import (
  "fmt"
  "os"
  "os/user"
  "runtime"
)
[
  user, _ := user.Current()
  fmt.Printf("Go: %s (%s_%s)\n", runtime.Version(), runtime(), runtime.GOOS, runtime.GOARCH)
  fmt.Printf("User:%s\n", user.Username)
  wd, _ := os.Getwd()
  fmt.Printf("Working dir: %s\n", wd)
  fmt.Printf("NumCPU: %d\n", runtime.NumCPU())
]

func naiveFib(n int) int {
  if n > 1 {
    return naiveFib(n - 1) + naiveFib(n - 2)
  }
  return 1
}

import "fmt"
 
n := 10

if n > 0 {
  fmt.Println("n is positive:", n)
}else {
  fmt.Println("n is not positive:", n)
}

sum := 0
for i := 1; i <= n; i++ {
  sum += i
}
sum

switch sum {
case 55:
  fmt.Println("OK")
default:
  fmt.Println("Fail")
}

import (
  "fmt"
  "math"
)

import (
  "bytes"
  "fmt"
  "image"
  png "image/png"
  jpeg "image/jpeg"
  "os"
  "time"
  
  "github.com/nfnt/resize"
)
[
 img, err := png.Decode(bytes.NewBuffer(gopherPNG))
 if err != nil {
   fmt.Fprintf(os.Stderr, "Failed to decode:", err)
   return
 }
 img = resize.Resize(100, 0, img, resize.Lanczos3)
 var labelID, imgID string
 for quality := 25; quality > 0; quality -= 1 [
   var buf bytes.Buffer
   jpeg.Encode (&buf, img, &jpeg.Options{Quality: quality})
   size := float32(len(buf.Bytes()))/1000
   _ctx.Display.Text(fmt.Sprintf("Quality: %d\nSize: %.2fkB", quality, size), &labelID)
   time.Sleep(200*time.Millisecond)
 ]
]
```

```
git clone https://github.com/yunabe/lgo.git
cd lgo/docker/jupyter
docker-compose up -d

docker-compose exec jupyter jupyter notebook list

./up.sh
./down.sh

cd $GOPATH/src; go install ./...
multiple roots $LGOPATH/pkg 
lgo run
```

```go
b := make([]byte, 1 << 25)

b := make([]byte, 1 << 25)

b = nil

a, b := 3, 4

func sum(x, y int) int {
  return x + y
}

import "fmt"

fmt.Sprintf("sum(%d, %d) = %d", a, b, sum(a, b))
sum(3, 4) = 7
```


