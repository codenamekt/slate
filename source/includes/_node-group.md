# Node Group

```golang
type NodeGroup struct {
    gorm.Model
    NodeFlavor NodeFlavor `json:"node_flavor" db:"node_flavor"`
    Count int `json:"count" db:"count"`
    Cluster Cluster `json:"cluster" db:"cluster"`
    NodeRole int `json:"node_role" db:"node_role"`
}
```