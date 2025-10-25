<img src= "https://github.com/thrushlang/.github/blob/main/assets/logos/thrushlang-logo.png" alt= "logo" style= "width: 80%; height: 80%;"></img>

# The Thrush Quantum Compiler 

The **Thrush Quantum Compiler** transfers source code from Quantum Thrush ``.thrushq`` files directly into an intermediate IR that is portable to the quantum counterpart. The process includes static type analysis, code generation, target-specific optimizations, and interpretation.

> [!IMPORTANT]  
> This compiler is in the placeholder phase and has not yet started development.

# Compiler Backends

<div align= "center">
  <img src= "https://github.com/qir-alliance/.github/blob/main/logo/alliance/white/teal_highres.png" alt= "qirlogo" style= "width: 30%; height: 30%;"></img>
  <h2>Quantum Intermediate Representation (QIR)</h2>
</div>

The Quantum Intermediate Representation (QIR) is a standardized intermediate representation based on LLVM IR, developed collaboratively by the QIR Alliance, which includes industry leaders such as Microsoft, NVIDIA, Quantum Computing Inc. (QCI), and Quantinuum.

QIR aims to provide a unified framework for quantum computing, enabling the generation of portable and interoperable code across various quantum hardware and simulators. It serves as a bridge between high-level quantum programming languages, such as Microsoft’s Q#, and low-level quantum instructions, enabling the compilation or emulation of quantum programs into valid quantum representations executable on quantum processors or classical simulators.

The Thrush Quantum Compiler, designed for the Thrush programming language quantum domain-specific language (DSL) `.thrushq` or `.⚛️🐦` is being developed to integrate QIR as its primary intermediate representation. Thrush will generate a custom LLVM-based IR that adheres to the QIR specification, enabling compilation of Thrush programs into quantum circuits or instructions compatible with various quantum backends. This integration, planned for a future release, will require a significant rewrite of both the frontend and the backend of the current __**[Thrush Compiler](https://github.com/thrushlang/thrushc)**__.

Much of the QIR Alliance infrastructure is built on Rust, making it easy to integrate with the future of the compiler.

By adopting QIR, Thrush aims to improve its interoperability, using the QIR Alliance Rust-based infrastructure, and provide a robust platform for developing quantum algorithms, offering functionality similar to Q#.

For more details of QIR Alliance: https://github.com/qir-alliance
