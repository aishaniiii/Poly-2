# Poly-2

---

## Hardhat-Circom Template for Circuit Development

### Overview

This project utilizes a Hardhat-Circom template to facilitate the development of a zero-knowledge proof circuit. The goal is to create a circuit that can be compiled, generate proofs, and deploy a verifier contract on a testnet.

### Project Rubric

To successfully complete the Final Challenge, the following steps need to be executed:

1. **Circuit Implementation**: Write a correct `circuit.circom` implementation. This involves defining the circuit's logic and constraints.

2. **Compilation**: Compile the circuit to generate necessary intermediaries such as the `.json` representation of the circuit.

3. **Proof Generation**: Generate a proof using specific inputs. For this project, the proof should be generated with inputs `A=0` and `B=1`.

4. **Verifier Contract Deployment**: Deploy a solidity verifier contract. This verifier should be capable of verifying the proof generated by the circuit.

5. **Verification**: Call the `verifyProof()` method on the deployed verifier contract and assert that the output is `true`, indicating successful verification of the proof.

### Steps to Execute

1. **Setup**

   - Clone this repository to your local machine.
   - Ensure you have Node.js (recommended version 14.x) and npm installed.

2. **Install Dependencies**

   ```bash
   npm install
   ```

3. **Development Workflow**

   - **Circuit Design**: Edit the `circuit.circom` file located in the `circuits` directory. Define your circuit's logic here.
   
   - **Compilation**: Use Hardhat to compile the circuit. Run:
     
     ```bash
     npx hardhat compile
     ```

   - **Proof Generation**: Generate a proof with specified inputs `A=0` and `B=1`. This typically involves using Circom or related tooling specific to your setup.

   - **Verifier Deployment**: Deploy the verifier contract to Sepolia or Mumbai Testnet. Modify the deployment scripts (`deploy.js` or similar) as per your requirements.

   - **Verification**: After deploying the verifier contract, interact with it using a script or through a UI (like Remix). Call the `verifyProof()` method with the generated proof and verify that the output is `true`.

4. **Testing**

   - Include comprehensive testing to validate each component's functionality. Ensure that the circuit behaves correctly, proofs are generated and verified as expected, and the verifier contract operates correctly.

5. **Deployment**

   - Deploy the finalized solution, including the circuit, proofs, and verifier contract, to your chosen testnet environment.

### Resources

- [Hardhat](https://hardhat.org/) for Ethereum development and testing.
- [Circom](https://github.com/iden3/circom) for circuit design and compilation.
- Solidity for writing the verifier contract.
- Sepolia or Mumbai Testnet for deploying and testing smart contracts.

### Conclusion

This README serves as a guide to developing a zero-knowledge proof circuit using the Hardhat-Circom template. Follow the outlined steps to meet the project requirements and achieve successful completion of the Final Challenge.

For any questions or issues, please refer to the documentation of the tools mentioned or reach out to the community for support.

--- 
