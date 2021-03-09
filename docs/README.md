@amplitude/react-native / [Exports](modules.md)

# @amplitude/react-native

Official Amplitude React Native SDK

```diff
! v2 of this SDK is newly developed and has just been released.  Please file any bug reports under issues. PR's welcome!
```

## Installation

```sh
yarn add @amplitude/react-native
```

## Documentation

[Exported Modules](docs/modules.md)

## Usage

```tsx
import * as React from 'react';
import { Button } from 'react-native';
import { Amplitude, Identify } from '@amplitude/react-native';

const ampInstance = Amplitude.getInstance();
ampInstance.init(API_KEY);

export function MyApp() {
  return (
    <Button
      title="Log Event"
      onPress={() => ampInstance.logEvent('BUTTON_CLICKED')}
    />
  );
}
```

## Contributing

See the [contributing guide](CONTRIBUTING.md) to learn how to contribute to the
repository and the development workflow.

## License

MIT