# Spanish Community Flags 🇪🇸

Welcome to `spanish-community-flags`, a versatile Vue component that renders the flags of Spanish communities based on ISO codes. Whether you want to showcase Spanish regional pride, illustrate data, or create a community-centered UI, this component has got you covered.

## Features 🌟

- 🚩 Supports all 17 autonomous communities in Spain.
- 💡 Toggle flag names on or off.
- 🎨 Highly customizable with CSS.

## Installation 📦

Using npm:

```bash
npm install git+https://github.com/jrondon/p0-spanish-community-flags.git
```

Or using yarn:

```bash
yarn add https://github.com/jrondon/p0-spanish-community-flags.git
```
## Usage 🛠️

1. **Import the Component**: 

   First, ensure that the component is imported in your Vue component or view:
   
```javascript
import SpanishCommunityFlags from 'spanish-community-flags'
```

2. **Register the Component**:

If you're using it within a Vue component, make sure to register it:

   
```javascript
components: {
  SpanishCommunityFlags
}
```

3. **Use the Component**:

Add the `SpanishCommunityFlags` component to your template. Specify the desired ISO code and toggle the name display as needed:

```javascript
<SpanishCommunityFlags :isoCode="o.code" :showName="false" class="mr-2 w-[20px] border" />
```

## Props 🔄
| Prop      | Type    | Default | Description                                 |
|-----------|---------|---------|---------------------------------------------|
| `isoCode` | String  | none    | ISO code of the Spanish community.          |
| `showName`| Boolean | true    | Whether to display the name of the community |



## Styling 💄
The component is designed to be styled with your desired CSS classes or styles. Use them to fit the component into your design theme seamlessly.

## Contributing 🤝
We appreciate any contribution to improve `spanish-community-flags`. Please make sure to read our contribution guidelines before making a PR.

## License 📄
This project is licensed under the MIT License.

