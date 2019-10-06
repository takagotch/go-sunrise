### go-sunrise
---
https://github.com/nathan-osman/go-sunrise

```go
// center_test.go

var dataEquationOfCenter []struct {
  in float64
  out float64
}{
  {358.30683, -0.05778},
  {357.7462, -0.0769},
  {87.16704, 1.91414},
}

func TestEquationOfCenter(t *testing.T) {
  for _, tt := range dataEquationOfCenter {
    v := EquationOfCenter(tt.in)
    if Round(v, DefaultPlaces) != Round(tt.out, DefaultPlaces) {
      t.Fatalf("%f != %f", v, tt.out)
    }
  }
}
```

```
```

```
```


