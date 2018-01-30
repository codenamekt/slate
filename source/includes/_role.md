# Role

```golang
type Role struct {
    gorm.Model
    Name string `json:"name" db:"name"`
}
```