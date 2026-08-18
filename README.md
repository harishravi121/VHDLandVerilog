# VHDLandVerilog
Lots of VHDL and verilog code
module toplevel(clock,reset);
  input clock;
  input reset;

  reg flop1;
  reg flop2;

  always @ (posedge reset or posedge clock)
    if (reset)
      begin
        flop1 <= 0;
        flop2 <= 1;
      end
    else
      begin
        flop1 <= flop2;
        flop2 <= flop1;
      end
endmodule


Hi folks here is fpga vs microcontroller.. I have coded both.. with FPGA you need  12 GB install software and Micro only 300 Mb so micro is great for massproducing utilities.. However every time you manufacture a processor for smartphone or pc you need to know some verilog or vhdl
teaching that is also a good job.. I wanted to buy fpga in 2008 and teach all hostel mates but didnt till 2015 there too never taught on board like a Phd in Elec..
