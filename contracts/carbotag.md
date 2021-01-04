# CarboTag

## `CarboTag`

You can use this contract for transacting carbon credits.

Contract which executes trade between 2 entities via escrow.

## Functions:

* [`getEscrowList(address _address)`](carbotag.md#CarboTag-getEscrowList-address-)
* [`constructor(address factory, address payable oldAddr)`](carbotag.md#CarboTag-constructor-address-address-payable-)
* [`fallback()`](carbotag.md#CarboTag-fallback--)
* [`addGovernor(address _target)`](carbotag.md#CarboTag-addGovernor-address-)
* [`signUp(string name)`](carbotag.md#CarboTag-signUp-string-)
* [`findEscrowAddr(address _sender, address _receiver)`](carbotag.md#CarboTag-findEscrowAddr-address-address-)
* [`createEscrow(address _receiver)`](carbotag.md#CarboTag-createEscrow-address-)
* [`addCarbon(uint256 carbon)`](carbotag.md#CarboTag-addCarbon-uint256-)
* [`createTransaction(address _receiver, int256 _carbon, int256 _gold)`](carbotag.md#CarboTag-createTransaction-address-int256-int256-)
* [`acceptTransaction(address _sender, address _receiver, uint256 _txID, int256 _carbon, int256 _gold)`](carbotag.md#CarboTag-acceptTransaction-address-address-uint256-int256-int256-)
* [`rejectTransaction(address _counterparty, uint256 _txID)`](carbotag.md#CarboTag-rejectTransaction-address-uint256-)
* [`addStamper(address target, uint256 stamprate, uint256 minpmt)`](carbotag.md#CarboTag-addStamper-address-uint256-uint256-)
* [`updateGold(uint256 stamps, address stamper)`](carbotag.md#CarboTag-updateGold-uint256-address-)
* [`transactionData(address _escrowAddr, uint256 _txID)`](carbotag.md#CarboTag-transactionData-address-uint256-)
* [`getTransactionIds(address _escrowAddr, uint256 from, uint256 to)`](carbotag.md#CarboTag-getTransactionIds-address-uint256-uint256-)
* [`changeOwner(address _newOwner)`](carbotag.md#CarboTag-changeOwner-address-)
* [`killContract()`](carbotag.md#CarboTag-killContract--)

## Events:

* [`EscrowFunded(address sender, uint256 value)`](carbotag.md#CarboTag-EscrowFunded-address-uint256-)

## getEscrowList

### No description

#### `getEscrowList(address _address) → address[]` <a id="CarboTag-getEscrowList-address-"></a>

## constructor

### No description

#### `constructor(address factory, address payable oldAddr)` <a id="CarboTag-constructor-address-address-payable-"></a>

## fallback

### No description

#### `fallback()` <a id="CarboTag-fallback--"></a>

## addGovernor

### No description

#### `addGovernor(address _target)` <a id="CarboTag-addGovernor-address-"></a>

## signUp

### No description

#### `signUp(string name)` <a id="CarboTag-signUp-string-"></a>

## findEscrowAddr

### No description

#### `findEscrowAddr(address _sender, address _receiver) → address payable _escrow` <a id="CarboTag-findEscrowAddr-address-address-"></a>

## createEscrow

### create a escrow account with you and the receiver

#### `createEscrow(address _receiver) → address payable _escrowAddr` <a id="CarboTag-createEscrow-address-"></a>

### Parameters:

* `_receiver`: The receiver account

### Return Values:

* Escrow Address

## addCarbon

### No description

#### `addCarbon(uint256 carbon)` <a id="CarboTag-addCarbon-uint256-"></a>

## createTransaction

### No description

#### `createTransaction(address _receiver, int256 _carbon, int256 _gold)` <a id="CarboTag-createTransaction-address-int256-int256-"></a>

## acceptTransaction

### No description

#### `acceptTransaction(address _sender, address _receiver, uint256 _txID, int256 _carbon, int256 _gold)` <a id="CarboTag-acceptTransaction-address-address-uint256-int256-int256-"></a>

## rejectTransaction

### No description

#### `rejectTransaction(address _counterparty, uint256 _txID)` <a id="CarboTag-rejectTransaction-address-uint256-"></a>

## addStamper

### No description

#### `addStamper(address target, uint256 stamprate, uint256 minpmt)` <a id="CarboTag-addStamper-address-uint256-uint256-"></a>

## updateGold

### No description

#### `updateGold(uint256 stamps, address stamper)` <a id="CarboTag-updateGold-uint256-address-"></a>

## transactionData

### No description

#### `transactionData(address _escrowAddr, uint256 _txID) → uint256` <a id="CarboTag-transactionData-address-uint256-"></a>

## getTransactionIds

### No description

#### `getTransactionIds(address _escrowAddr, uint256 from, uint256 to) → uint256[] _transactionIds` <a id="CarboTag-getTransactionIds-address-uint256-uint256-"></a>

## changeOwner

### No description

#### `changeOwner(address _newOwner)` <a id="CarboTag-changeOwner-address-"></a>

## killContract

### No description

#### `killContract()` <a id="CarboTag-killContract--"></a>

## Event `EscrowFunded(address sender, uint256 value)` <a id="CarboTag-EscrowFunded-address-uint256-"></a>

No description

