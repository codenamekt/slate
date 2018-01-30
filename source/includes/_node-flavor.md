# Node Flavor

```golang
type NodeFlavor struct {
    gorm.Model
    InstanceType string `json:"instance_type" db:"instance_type"`
    Product Product `json:"product" db:"product"`
    Provider Provider `json:"provider" db:"provider"`
    Name string `json:"name" db:"name"`
    Version string `json:"version" db:"version"`
}
```