# Vesting Contract

This project includes a smart contract for managing token vesting with role-based access control and a front-end interface built with React.

## Smart Contract

### Roles

- **User**: 50% of total allocated tokens with a cliff of 10 months and a total vesting duration of 2 years.
- **Partners**: 25% of total allocated tokens with a cliff of 2 months and a total vesting duration of 1 year.
- **Team**: 25% of total allocated tokens with a cliff of 2 months and a total vesting duration of 1 year.

### Features

- Allow the owner to start vesting.
- Enable the addition of beneficiaries for each role before vesting starts.
- Allow beneficiaries to claim their vested tokens according to the schedule.
- Track and emit events for vesting start, beneficiary addition, and token withdrawal.

### Testing

- Test the creation of vesting schedules by the admin.
- Verify proper token claiming by beneficiaries according to the schedule.
- Ensure the correct calculation of vested tokens based on cliff and duration.

## Front-End Interface

The front-end is built using React and Web3.js to interact with the smart contract.

### Setup

1. Clone the repository.
2. Install dependencies: `npm install`.
3. Start the development server: `npm start`.

### Usage

- Start the vesting process by clicking "Start Vesting".
- Add beneficiaries by entering their address, role, and amount.
- Beneficiaries can claim their tokens by entering their role and clicking "Claim Tokens".

## Deployment

Deploy the smart contract using Hardhat or Truffle and update the contract address in the front-end configuration.

## License

This project is licensed under the MIT License.
