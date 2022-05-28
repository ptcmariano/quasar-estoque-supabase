# Quasar Estoque Supabase (quasar-estoque-supabase)

Project built on the Youtube Quasar + Supabase course: [Playlist on Youtube](https://www.youtube.com/watch?v=6ep8cy6pP74&list=PLBjvYfV_TvwIfgvouZCaLtgjYdrWQL02d&index=1)

## Init Config

You are required to configure the ***quasar.conf.js*** file with your supabase credentials.

```js
build: {
  env: {
    SUPABASE_URL: 'XXXX',
    SUPABASE_KEY: 'YYYY'
  }
}
```

## Install the dependencies
```bash
yarn
```

### Start the app in development mode (hot-code reloading, error reporting, etc.)
```bash
quasar dev
```

### Lint the files
```bash
yarn run lint
```

### Build the app for production
```bash
quasar build
```

### On supabase create tables
```sql
CREATE TABLE category AS
    select '' as user_id, '' as name WITH NO DATA;
CREATE TABLE product AS
    select '' as user_id, '' as name, '' as description
           '' as img_url, 1 as category_id, 1 as price, 0.1 as amount
            WITH NO DATA;
CREATE TABLE category AS
    select '' as user_id, '' as name, '' as paralax_url,
            '' as phone, '' as primary, '' as secondary
             WITH NO DATA;
```

### Customize the configuration
See [Configuring quasar.conf.js](https://quasar.dev/quasar-cli/quasar-conf-js).
