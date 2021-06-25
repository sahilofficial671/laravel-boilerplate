# Laravel Boilerplate
Simple laravel essentials to kik start your new project. :rocket:

### Features

- Fortify Authentication :lock:
    - Login & Registration
    - Email Verification
    - Reset Password

- Views with components for Frontend :heart:
    - Dashboard

- Tailwind CSS, Alpine.js, Laravel Mix, Axios :art:

## Components
- [Button](#button)

## Button

###  Type
```vue
<x-button buttonType="primary" />
```

> Default: `primary`

##### Common Classes:
```css 
inline-flex py-2 items-center border border-transparent rounded-md font-semibold text-xs uppercase tracking-widest focus:outline-none focus:ring disabled:opacity-25 transition ease-in-out duration-150 shadow-sm
```
##### Available Options:
```css
primary        => bg-blue-600 text-white ring-blue-200 focus:border-blue-700 active:bg-blue-700
secondary      => bg-indigo-100 border-indigo-200 border-opacity-60 text-indigo-700 ring-indigo-200 focus:border-indigo-300 active:bg-indigo-900
danger         => bg-red-600 text-white ring-red-200 focus:border-red-700 active:bg-red-700
danger-light   => bg-red-200 text-red-600 ring-red-200 focus:border-red-300 active:bg-red-300 border-red-300 border-opacity-60
light          => bg-gray-200 text-gray-600 ring-gray-200 focus:border-gray-300 active:bg-gray-300
light-success  => bg-green-200 text-green-600 ring-green-200 focus:border-green-300 active:bg-green-300 border-green-300 border-opacity-60
```

###  Height
```vue
<x-button height="h-14" />
```

> Default: `h-10`
