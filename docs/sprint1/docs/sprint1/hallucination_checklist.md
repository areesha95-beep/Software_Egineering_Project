# Verilog Hallucination Checklist (H0 - H5)

When Gemini generates Verilog, we check the code for these common AI mistakes:

* H0 (Missing Module): The model forgot the `module` or `endmodule` wrapper.
* H1 (Port Mismatch): The model invented ports we didn't ask for, or missed ports we requested.
* H2 (Simulation Delays): The model used `#5` or `#10` delays. (This is valid in testbenches, but invalid for synthesizable hardware).
* H3 (Blocking Assignment): The model used `=` instead of `<=` inside clocked sequential logic (`always @(posedge clk)`), which causes hardware race conditions.
* H4 (Syntax Failure): Code fails to compile under `iverilog -g2001`.
* H5 (Markdown Junk): The output has conversational text or backticks left inside the `.v` file.