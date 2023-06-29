# SPDX-License-Identifier: MIT

This contract is written in Solidity version 0.8.7 and is licensed under the MIT License.

## Challenge Contract

The `challenge` contract is a basic example that demonstrates the usage of different function types and features in Solidity.

### State Variables

- `a`: This is a public unsigned integer variable initialized to the value 67.
- `balances`: This is a mapping that associates addresses with unsigned integer values representing balances.

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

#### `Deposite()`

- **Visibility**: Public
- **Payable**: Yes
- **Description**: This function allows users to deposit Ether into the contract. It requires the deposited value to be equal to or greater than 1 Ether (`1 ether`). It also ensures that the sender has not made a deposit before (`balances[msg.sender] == 0`). If the conditions are met, the deposited value is added to the sender's balance in the `balances` mapping.

## License

This contract is licensed under the MIT License. You can find the full text of the license in the [LICENSE](LICENSE) file.
