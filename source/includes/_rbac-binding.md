# RBAC Binding

```golang
type RBACBinding struct {
    gorm.Model
    Name string `json:"name" db:"name"`
    Type int `json:"type" db:"type"`
    Groups []string `json:"groups" db:"groups"`
}
```