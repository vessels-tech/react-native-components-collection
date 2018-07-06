# `<MapView />` Component API

## Dependencies

#### react-native-maps > 0.21

## Children

⚠ A chaque Marker Custom ajouter les props:

- id
- coordinate : { longitude, latitude }

## Props

### Props from the [react-native-maps API](https://github.com/react-community/react-native-maps/blob/master/docs/mapview.md)

### Other props

| Prop | Type | Default | Note |
|---|---|---|---|
| `clustering` | `boolean` | False | (Optional) When true enables clustering of Markers.
| `renderCluster` |`(Cluster) => React.Node` | Renders default clusters on Map | (Optional) Render your custom clusters.
| `onPressCluster` | `(Cluster) => void` | onPress not handled | (Optional) Handle onPress on default clusters.


## Types

```
type Cluster {
  properties : {
    cluster: Boolean
    cluster_id: Number
    point_count: Number
    point_count_abbreviated: String
  }
  geometry: {
    coordinates: [(longitude), (latitude)]
  }
}
```