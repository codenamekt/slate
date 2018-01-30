# Cluster

```golang
type Cluster struct {
    gorm.Model
    Name string `json:"name" db:"name"`
    Account Account `json:"account" db:"account"`
    Region Region `json:"region" db:"region"`
    Version string `json:"version" db:"version"`
    TargetVersion string `json:"target_version" db:"target_version"`
    State string `json:"state" db:"state"`
    Provider Provider `json:"provider" db:"provider"`
    Credential string `json:"credential" db:"credential" platform_team:"do_we_need"`
}
```