# Product

```golang
type Product struct {
    gorm.Model
    Name string `json:"name" db:"name"`
}
```