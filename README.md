[![npm](https://img.shields.io/npm/v/@swenkerorg/possimus-ullam-laudantium.svg)](https://www.npmjs.com/package/@swenkerorg/possimus-ullam-laudantium) ![downloads](https://img.shields.io/npm/dt/@swenkerorg/possimus-ullam-laudantium.svg) [![CI](https://github.com/swenkerorg/possimus-ullam-laudantium/actions/workflows/ci.yml/badge.svg)](https://github.com/swenkerorg/possimus-ullam-laudantium/actions)

# Make-Event-Props

A function that, given props, returns an object of event callback props optionally curried with additional arguments.

This package allows you to pass event callback props to a rendered DOM element without the risk of applying any invalid props that could cause unwanted side effects.

## tl;dr

- Install by executing `npm install @swenkerorg/possimus-ullam-laudantium` or `yarn add @swenkerorg/possimus-ullam-laudantium`.
- Import by adding `import makeEventProps from '@swenkerorg/possimus-ullam-laudantium'`.
- Create your event props object:
  ```ts
  const eventProps = useMemo(
    () => makeEventProps(props, (eventName) => additionalArgs),
    [additionalArgs],
  );
  ```
- Use your event props:
  ```tsx
  return <div {...eventProps} />;
  ```

## License

The MIT License.

## Author

<table>
  <tr>
    <td >
      <img src="https://avatars.githubusercontent.com/u/5426427?v=4&s=128" width="64" height="64" alt="Wojciech Maj">
    </td>
    <td>
      <a href="https://github.com/wojtekmaj">Wojciech Maj</a>
    </td>
  </tr>
</table>
