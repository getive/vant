## Pagination

### Install
``` javascript
import { Pagination } from 'vant';

Vue.use(Pagination);
```

### Usage

#### Basic Usage

```html
<van-pagination 
  v-model="currentPage" 
  :total-items="24" 
  :items-per-page="5"
/>
```

```javascript
export default {
  data() {
    return  {
      currentPage: 1
    }
  }
}
```

#### Simple mode

```html
<van-pagination 
  v-model="currentPage" 
  :page-count="12"
  mode="simple" 
/>
```

#### Show ellipses

```html
<van-pagination 
  v-model="currentPage" 
  :total-items="125" 
  :show-page-size="3" 
  force-ellipses
/>
```

### API

| Attribute | Description | Type | Default | Accepted Values |
|-----------|-----------|-----------|-------------|-------------|
| v-model | Current page number | `Number` | - | - |
| mode | Mode | `String` | `multi` | `simple`  |
| items-per-page | Item number per page | `Number` | `10` | - |
| prev-text | Previous text | `String` | `Previous` | - |
| next-text | Next text | `String` | `Next` | - |
| show-page-size | Count of page size to show | `Number` | `5` | - |
| force-ellipses | Whether to show ellipses | `Boolean` | `false` | - |

### Event

| Event | Description | Attribute |
|-----------|-----------|-----------|
| change | Triggered on page change | - |
