# Region

```golang
type Region struct {
    gorm.Model
    Name string `json:"name" db:"name"`
    Provider Provider `json:"provider" db:"provider"`
    Enabled bool `json:"enabled" db:"enabled"`
}
```