<img src= "https://github.com/thrushlang/.github/blob/main/assets/logos/thrushlang-logo.png" alt= "logo" style= "width: 80%; height: 80%;"></img>

# The Quantum Thrush Compiler 

The **Quantum Thrush Compiler** transfers source code from Quantum Thrush ``.thrushq`` files directly into an intermediate IR that is portable to the quantum counterpart. The process includes static type analysis, code generation, target-specific optimizations, and interpretation.

> [!IMPORTANT]  
> This compiler is in the placeholder phase and has not yet started development.

# Compiler Backends

<div aling= "center">
  <img src= "https://github.com/qir-alliance/.github/blob/main/logo/alliance/white/teal_highres.png" alt= "qirlogo" style= "width: 70%; height: 70%;"></img>
  <h2>Quantum Intermediate Representation (QIR)</h2>
</div>


It is a backend compiler collaboratively developed by multiple companies such as Microsoft, Nvidia, QCI, and Quantinuum to standardize code generation for quantum computing, currently used by Q# to emulate or compile to a valid quantum representation.

Built with a specification based on LLVM IR.

Thrush will try to generate a specific IR for this backend, using LLVM tools.

This largely reassembles the functionality of Q#, but returns Thrush to being a quantum DSL.

It will include its bytecode runner and the QCOR compiler.

A significant portion of the QIR-Alliance infrastructure is written in Rust.

Its integration will happen in the future. Both the backend and the frontend need to be rewritten compared to __**[Thrush Compiler](https://github.com/thrushlang/thrushc)**__.
