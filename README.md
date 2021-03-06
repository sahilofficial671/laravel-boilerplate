# Laravel Boilerplate

![https://github.com/sahilofficial671/laravel-boilerplate/actions?query=workflow%3ABuild"](https://github.com/sahilofficial671/laravel-boilerplate/actions/workflows/build.yml/badge.svg)

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
- [Cards](#cards)
- [Modal](#modal)
- [Form components](#form-components)
    - [Input](#input)
    - [Select](#select)
    - [Textarea](#textarea)
    - [Datetime](#datetime)
- [Pill](#pill)
- [Back](#back)


## Button

####  Button Type
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

####  Height
```vue
<x-button height="h-14" />
```

> Default: `h-10`

####  Padding
```vue
<x-button padding="px-6 py-2" />
```

> Default: `px-2.5`

####  Value
```vue
<x-button value="Update" />
```

> Default: `// Empty`

## Cards

#### Header
```vue
<x-card>
    <x-slot name="header"> .. </x-slot>
</x-card>
```

#### Body
```vue
<x-card>
    <x-slot name="body"> .. </x-slot>
</x-card>
```

####  Width

```vue
<x-card width="sm:max-w-lg">
    ...
</x-card>
```
> Default: `sm:max-w-md`

##### Common Classes:
```css
w-full mt-2 sm:mt-4 md:mt-6 bg-white shadow-md overflow-hidden rounded-lg
```
## Form Components
## Input
####  Type

```vue
<x-input type="email" />
```

> Default: `text`

##### Common Classes:
```css 
shadow-sm border-gray-300 focus:ring focus:ring-opacity-50
```

##### Available Options:
```css
text     =>  rounded-md focus:border-blue-300 focus:ring-blue-200 text-gray-700
password =>  rounded-md focus:border-blue-300 focus:ring-blue-200 text-gray-700
number   =>  rounded-md focus:border-blue-300 focus:ring-blue-200 text-gray-700
email    =>  rounded-md focus:border-blue-300 focus:ring-blue-200 text-gray-700
checkbox =>  rounded h-5 w-5 checked:text-blue-600 checked:border-transparent text-blue-600 focus:outline-none focus:ring-blue-200 cursor-pointer
```

## Select

```vue
<x-select> ... </x-select>
```

##### Common Classes:
```css 
w-full shadow-sm border-gray-300 focus:ring focus:ring-opacity-50 rounded-md focus:border-blue-300 focus:ring-blue-200 cursor-pointer
```

## Textarea
```vue
<x-textarea> ... </x-textarea>
```

####  Type

```vue
<x-textarea value="This is textarea value." />
<x-textarea value="This is textarea value."> ... </x-textarea>
```

##### Common Classes:
```css 
rounded-md shadow-sm border-gray-300 focus:border-blue-300 focus:ring focus:ring-blue-200 focus:ring-opacity-50
```

## DateTime
```vue
<x-datetime> ... </x-datetime>
```

####  Type

```vue
<x-datetime type="date_type_name" />
```

> Default: `text`

####  isHidden

```vue
<x-datetime isHidden="true|false" />
```
> Default: `false`

####  Placeholder

```vue
<x-datetime placeholder="Select schedule date" />
```

> Default: `Select date`

####  Value

```vue
<x-datetime value="value for input field" />
```

> Default: `empty|blank`


##### Common Classes:
```css 
w-full shadow-sm border-gray-300 focus:ring focus:ring-opacity-50 rounded-md focus:border-green-300 focus:ring-green-200 text-sm text-gray-700 cursor-pointer
```


## Back

Back button used by user to go to previous page Ex: `< Back `
```vue
<x-back />
```

####  Value

```vue
<x-back value="Go back" /> 
```
Output: `< Go back`

> Default: `Back`

##### Common Classes:
```css 
ml-2 items-center hover:bg-gray-50 bg-opacity-50 rounded inline-flex
```

##### Text Classes:
```css
text-sm text-gray-600 hover:text-gray-900
```

## Modal
```vue
<x-modal> ... </x-modal>
```

####  Type

```vue
<x-modal type="warning" />
```

> Default: `info`
> Base icon for modal will also be added according to type of modal

##### Available Options:
```css
info      =>  icon_classes => text-blue-600,  'icon_container_class' => 'bg-blue-100'
danger    =>  icon_classes => text-red-600,  'icon_container_class' => 'bg-red-100'
warning   =>  icon_classes => text-yellow-600,  'icon_container_class' => 'bg-yellow-100'
success   =>  icon_classes => text-green-600, 'icon_container_class' => 'bg-green-100'  
```

####  Default Cancel

```vue
<x-modal defaultCancel="false" />
```

> Default: `true`
> It will show/hide default cancel text

####  Default Cancel Texh

```vue
<x-modal defaultCancelText="Close" />
```

> Default: `Cancel`
> It will change default cancel text

####  Toggle

```vue
<x-modal toggle="toggleable_value | {{ toggleable_value }}" />
```

> Default: `false`
> Toggle key helps cancel button to hide modal.

####  Header

```vue
<x-modal toggle="toggleable_value type="success">
    <x-slot name="header">
        ...
    </x-slot>
</x-modal>
```

####  Body

```vue
<x-modal toggle="toggleable_value type="success">
    <x-slot name="body">
        ...
    </x-slot>
</x-modal>
```

## Pill
```vue
<x-pill> ... </x-pill>
```

####  Type

```vue
<x-pill type="warning" />
```

> Default: `info`

##### Available Options:
```css
info      =>  bg-indigo-100 text-indigo-600,
danger    =>  bg-red-100 text-red-600,
warning   =>  bg-yellow-100 text-yellow-600,
success   =>  bg-green-100 text-green-600,
```

####  Value

```vue
<x-pill value="Mobile" />
```

> Default: `Information`

##### Common Classes:
```css
text-xs font-semibold p-1 rounded-md
```

