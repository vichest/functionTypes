# functionTypes
write a smart contract that uses view, pure, and payable functions. Ensure that the functions are accessible within the contract and derived contracts as well.
# SPDX-License-Identifier: MIT

This contract is written in Solidity version 0.8.7 and is licensed under the MIT License.

## Challenge Contract

The `challenge` contract is a basic example that demonstrates the usage of different function types in Solidity.

### State Variable

- `a`: This is a public unsigned integer variable initialized to the value 67.

### Functions

#### `typePure(uint c, uint b)`

- **Type**: Pure function
- **Visibility**: Public
- **Parameters**:
  - `c`: Unsigned integer parameter
  - `b`: Unsigned integer parameter
- **Returns**: Unsigned integer
- **Description**: This pure function calculates the sum of `c` and `b` and returns the result.

#### `typeView(uint b)`

- **Type**: View function
- **Visibility**: Public
- **Parameters**:
  - `b`: Unsigned integer parameter
- **Returns**: Unsigned integer
- **Description**: This view function adds the value of the state variable `a` to `b` and returns the result. It does not modify the state of the contract.

## License

This contract is licensed under the MIT License. You can find the full text of the license in the [LICENSE](LICENSE) file.
