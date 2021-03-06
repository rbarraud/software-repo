Z80 Opcode Assembler / Disassembler||||||||||||
|-----------------------------------|------|------|------|------|------|------|------|------|-------|--------|-------------------------------------------------------------|
|Mnemonic                           |S     |Z     |H     |P     |N     |C     |Opcode|Data  |Suffix |T-States|Notes                                                        |
|ADC A,(HL)                         |*     |*     |*     |V     |0     |*     |8E    |      |       |7       |Add with carry location (HL) to acccumulator.                |
|ADC A,(IX+n)                       |*     |*     |*     |V     |0     |*     |DD 8E |XX    |       |19      |Add with carry location (IX+N) to accumulator.               |
|ADC A,(IY+n)                       |*     |*     |*     |V     |0     |*     |FD 8E |XX    |       |19      |Add with carry location (IY+N) to accumulator.               |
|ADC A,A                            |*     |*     |*     |V     |0     |*     |8F    |      |       |4       |Add with carry accumulator to itself.                        |
|ADC A,B                            |*     |*     |*     |V     |0     |*     |88    |      |       |4       |Add with carry register r to accumulator.                    |
|ADC A,C                            |*     |*     |*     |V     |0     |*     |89    |      |       |4       |Add with carry register r to accumulator.                    |
|ADC A,D                            |*     |*     |*     |V     |0     |*     |8A    |      |       |4       |Add with carry register r to accumulator.                    |
|ADC A,E                            |*     |*     |*     |V     |0     |*     |8B    |      |       |4       |Add with carry register r to accumulator.                    |
|ADC A,H                            |*     |*     |*     |V     |0     |*     |8C    |      |       |4       |Add with carry register r to accumulator.                    |
|ADC A,L                            |*     |*     |*     |V     |0     |*     |8D    |      |       |4       |Add with carry register r to accumulator.                    |
|ADC A,N                            |*     |*     |*     |V     |0     |*     |CE    |XX    |       |7       |Add with carry value n to accumulator.                       |
|ADC HL,BC                          |*     |*     |?     |V     |0     |*     |ED 4A |      |       |15      |Add with carry register pair BC to HL.                       |
|ADC HL,DE                          |*     |*     |?     |V     |0     |*     |ED 5A |      |       |15      |Add with carry register pair DE to HL.                       |
|ADC HL,HL                          |*     |*     |?     |V     |0     |*     |ED 6A |      |       |15      |Add with carry register pair HL to HL.                       |
|ADC HL,SP                          |*     |*     |?     |V     |0     |*     |ED 7A |      |       |15      |Add with carry register pair SP to HL.                       |
|ADD A,(HL)                         |*     |*     |*     |V     |0     |*     |86    |      |       |7       |Add location (HL) to acccumulator.                           |
|ADD A,(IX+n)                       |*     |*     |*     |V     |0     |*     |DD 86 |XX    |       |19      |Add location (IX+N) to accumulator.                          |
|ADD A,(IY+n)                       |*     |*     |*     |V     |0     |*     |FD 86 |XX    |       |19      |Add location (IY+N) to accumulator.                          |
|ADD A,A                            |*     |*     |*     |V     |0     |*     |87    |      |       |4       |Add register r to accumulator.                               |
|ADD A,B                            |*     |*     |*     |V     |0     |*     |80    |      |       |4       |Add register r to accumulator.                               |
|ADD A,C                            |*     |*     |*     |V     |0     |*     |81    |      |       |4       |Add register r to accumulator.                               |
|ADD A,D                            |*     |*     |*     |V     |0     |*     |82    |      |       |4       |Add register r to accumulator.                               |
|ADD A,E                            |*     |*     |*     |V     |0     |*     |83    |      |       |4       |Add register r to accumulator.                               |
|ADD A,H                            |*     |*     |*     |V     |0     |*     |84    |      |       |4       |Add register r to accumulator.                               |
|ADD A,L                            |*     |*     |*     |V     |0     |*     |85    |      |       |4       |Add register r to accumulator.                               |
|ADD A,N                            |*     |*     |*     |V     |0     |*     |C6    |XX    |       |7       |Add value n to accumulator.                                  |
|ADD HL,BC                          |      |      |?     |      |0     |*     |09    |      |       |11      |Add register pair BC to HL.                                  |
|ADD HL,DE                          |      |      |?     |      |0     |*     |19    |      |       |11      |Add register pair DE to HL.                                  |
|ADD HL,HL                          |      |      |?     |      |0     |*     |29    |      |       |11      |Add register pair HL to HL.                                  |
|ADD HL,SP                          |      |      |?     |      |0     |*     |39    |      |       |11      |Add register pair SP to HL.                                  |
|ADD IX,BC                          |      |      |?     |      |0     |*     |DD 09 |      |       |15      |Add register pair BC to IX.                                  |
|ADD IX,DE                          |      |      |?     |      |0     |*     |DD 19 |      |       |15      |Add register pair DE to IX.                                  |
|ADD IX,IX                          |      |      |?     |      |0     |*     |DD 29 |      |       |15      |Add register pair IX to IX.                                  |
|ADD IX,SP                          |      |      |?     |      |0     |*     |DD 39 |      |       |15      |Add register pair SP to IX.                                  |
|ADD IY,BC                          |      |      |?     |      |0     |*     |FD 09 |      |       |15      |Add register pair BC to IY.                                  |
|ADD IY,DE                          |      |      |?     |      |0     |*     |FD 19 |      |       |15      |Add register pair DE to IY.                                  |
|ADD IY,IY                          |      |      |?     |      |0     |*     |FD 29 |      |       |15      |Add register pair IY to IY.                                  |
|ADD IY,SP                          |      |      |?     |      |0     |*     |FD 39 |      |       |15      |Add register pair SP to IY.                                  |
|AND (HL)                           |*     |*     |*     |P     |0     |0     |A6    |      |       |7       |Logical AND of value at location (HL) to accumulator.        |
|AND (IX+n)                         |*     |*     |*     |P     |0     |0     |DD A6 |XX    |       |19      |Logical AND of value at location (IX+N) to accumulator.      |
|AND (IY+n)                         |*     |*     |*     |P     |0     |0     |FD A6 |XX    |       |19      |Logical AND of value at location (IY+N) to accumulator.      |
|AND A                              |*     |*     |*     |P     |0     |0     |A7    |      |       |4       |Logical AND of register r to accumulator.                    |
|AND B                              |*     |*     |*     |P     |0     |0     |A0    |      |       |4       |Logical AND of register r to accumulator.                    |
|AND C                              |*     |*     |*     |P     |0     |0     |A1    |      |       |4       |Logical AND of register r to accumulator.                    |
|AND D                              |*     |*     |*     |P     |0     |0     |A2    |      |       |4       |Logical AND of register r to accumulator.                    |
|AND E                              |*     |*     |*     |P     |0     |0     |A3    |      |       |4       |Logical AND of register r to accumulator.                    |
|AND H                              |*     |*     |*     |P     |0     |0     |A4    |      |       |4       |Logical AND of register r to accumulator.                    |
|AND L                              |*     |*     |*     |P     |0     |0     |A5    |      |       |4       |Logical AND of register r to accumulator.                    |
|AND N                              |*     |*     |*     |P     |0     |0     |E6    |XX    |       |7       |Logical AND of value n to accumulator.                       |
|BIT 0,(HL)                         |?     |*     |1     |?     |0     |      |CB 46 |      |       |12      |Test bit b of location (HL).                                 |
|BIT 0,(IX+n)                       |?     |*     |1     |?     |0     |      |DD CB |XX    |46     |20      |Test bit b of location (IX+N).                               |
|BIT 0,(IY+n)                       |?     |*     |1     |?     |0     |      |FD CB |XX    |46     |20      |Test bit b of location (IY+N).                               |
|BIT 0,A                            |?     |*     |1     |?     |0     |      |CB 47 |      |       |8       |Test bit b of register r.                                    |
|BIT 0,B                            |?     |*     |1     |?     |0     |      |CB 40 |      |       |8       |Test bit b of register r.                                    |
|BIT 0,C                            |?     |*     |1     |?     |0     |      |CB 41 |      |       |8       |Test bit b of register r.                                    |
|BIT 0,D                            |?     |*     |1     |?     |0     |      |CB 42 |      |       |8       |Test bit b of register r.                                    |
|BIT 0,E                            |?     |*     |1     |?     |0     |      |CB 43 |      |       |8       |Test bit b of register r.                                    |
|BIT 0,H                            |?     |*     |1     |?     |0     |      |CB 44 |      |       |8       |Test bit b of register r.                                    |
|BIT 0,L                            |?     |*     |1     |?     |0     |      |CB 45 |      |       |8       |Test bit b of register r.                                    |
|BIT 1,(HL)                         |?     |*     |1     |?     |0     |      |CB 4E |      |       |12      |Test bit b of location (HL).                                 |
|BIT 1,(IX+n)                       |?     |*     |1     |?     |0     |      |DD CB |XX    |4E     |20      |Test bit b of location (IX+N).                               |
|BIT 1,(IY+n)                       |?     |*     |1     |?     |0     |      |FD CB |XX    |4E     |20      |Test bit b of location (IY+N).                               |
|BIT 1,A                            |?     |*     |1     |?     |0     |      |CB 4F |      |       |8       |Test bit b of register r.                                    |
|BIT 1,B                            |?     |*     |1     |?     |0     |      |CB 48 |      |       |8       |Test bit b of register r.                                    |
|BIT 1,C                            |?     |*     |1     |?     |0     |      |CB 49 |      |       |8       |Test bit b of register r.                                    |
|BIT 1,D                            |?     |*     |1     |?     |0     |      |CB 4A |      |       |8       |Test bit b of register r.                                    |
|BIT 1,E                            |?     |*     |1     |?     |0     |      |CB 4B |      |       |8       |Test bit b of register r.                                    |
|BIT 1,H                            |?     |*     |1     |?     |0     |      |CB 4C |      |       |8       |Test bit b of register r.                                    |
|BIT 1,L                            |?     |*     |1     |?     |0     |      |CB 4D |      |       |8       |Test bit b of register r.                                    |
|BIT 2,(HL)                         |?     |*     |1     |?     |0     |      |CB 56 |      |       |12      |Test bit b of location (HL).                                 |
|BIT 2,(IX+n)                       |?     |*     |1     |?     |0     |      |DD CB |XX    |56     |20      |Test bit b of location (IX+N).                               |
|BIT 2,(IY+n)                       |?     |*     |1     |?     |0     |      |FD CB |XX    |56     |20      |Test bit b of location (IY+N).                               |
|BIT 2,A                            |?     |*     |1     |?     |0     |      |CB 57 |      |       |8       |Test bit b of register r.                                    |
|BIT 2,B                            |?     |*     |1     |?     |0     |      |CB 50 |      |       |8       |Test bit b of register r.                                    |
|BIT 2,C                            |?     |*     |1     |?     |0     |      |CB 51 |      |       |8       |Test bit b of register r.                                    |
|BIT 2,D                            |?     |*     |1     |?     |0     |      |CB 52 |      |       |8       |Test bit b of register r.                                    |
|BIT 2,E                            |?     |*     |1     |?     |0     |      |CB 53 |      |       |8       |Test bit b of register r.                                    |
|BIT 2,H                            |?     |*     |1     |?     |0     |      |CB 54 |      |       |8       |Test bit b of register r.                                    |
|BIT 2,L                            |?     |*     |1     |?     |0     |      |CB 55 |      |       |8       |Test bit b of register r.                                    |
|BIT 3,(HL)                         |?     |*     |1     |?     |0     |      |CB 5E |      |       |12      |Test bit b of location (HL).                                 |
|BIT 3,(IX+n)                       |?     |*     |1     |?     |0     |      |DD CB |XX    |5E     |20      |Test bit b of location (IX+N).                               |
|BIT 3,(IY+n)                       |?     |*     |1     |?     |0     |      |FD CB |XX    |5E     |20      |Test bit b of location (IY+N).                               |
|BIT 3,A                            |?     |*     |1     |?     |0     |      |CB 5F |      |       |8       |Test bit b of register r.                                    |
|BIT 3,B                            |?     |*     |1     |?     |0     |      |CB 58 |      |       |8       |Test bit b of register r.                                    |
|BIT 3,C                            |?     |*     |1     |?     |0     |      |CB 59 |      |       |8       |Test bit b of register r.                                    |
|BIT 3,D                            |?     |*     |1     |?     |0     |      |CB 5A |      |       |8       |Test bit b of register r.                                    |
|BIT 3,E                            |?     |*     |1     |?     |0     |      |CB 5B |      |       |8       |Test bit b of register r.                                    |
|BIT 3,H                            |?     |*     |1     |?     |0     |      |CB 5C |      |       |8       |Test bit b of register r.                                    |
|BIT 3,L                            |?     |*     |1     |?     |0     |      |CB 5D |      |       |8       |Test bit b of register r.                                    |
|BIT 4,(HL)                         |?     |*     |1     |?     |0     |      |CB 66 |      |       |12      |Test bit b of location (HL).                                 |
|BIT 4,(IX+n)                       |?     |*     |1     |?     |0     |      |DD CB |XX    |66     |20      |Test bit b of location (IX+N).                               |
|BIT 4,(IY+n)                       |?     |*     |1     |?     |0     |      |FD CB |XX    |66     |20      |Test bit b of location (IY+N).                               |
|BIT 4,A                            |?     |*     |1     |?     |0     |      |CB 67 |      |       |8       |Test bit b of register r.                                    |
|BIT 4,B                            |?     |*     |1     |?     |0     |      |CB 60 |      |       |8       |Test bit b of register r.                                    |
|BIT 4,C                            |?     |*     |1     |?     |0     |      |CB 61 |      |       |8       |Test bit b of register r.                                    |
|BIT 4,D                            |?     |*     |1     |?     |0     |      |CB 62 |      |       |8       |Test bit b of register r.                                    |
|BIT 4,E                            |?     |*     |1     |?     |0     |      |CB 63 |      |       |8       |Test bit b of register r.                                    |
|BIT 4,H                            |?     |*     |1     |?     |0     |      |CB 64 |      |       |8       |Test bit b of register r.                                    |
|BIT 4,L                            |?     |*     |1     |?     |0     |      |CB 65 |      |       |8       |Test bit b of register r.                                    |
|BIT 5,(HL)                         |?     |*     |1     |?     |0     |      |CB 6E |      |       |12      |Test bit b of location (HL).                                 |
|BIT 5,(IX+n)                       |?     |*     |1     |?     |0     |      |DD CB |XX    |6E     |20      |Test bit b of location (IX+N).                               |
|BIT 5,(IY+n)                       |?     |*     |1     |?     |0     |      |FD CB |XX    |6E     |20      |Test bit b of location (IY+N).                               |
|BIT 5,A                            |?     |*     |1     |?     |0     |      |CB 6F |      |       |8       |Test bit b of register r.                                    |
|BIT 5,B                            |?     |*     |1     |?     |0     |      |CB 68 |      |       |8       |Test bit b of register r.                                    |
|BIT 5,C                            |?     |*     |1     |?     |0     |      |CB 69 |      |       |8       |Test bit b of register r.                                    |
|BIT 5,D                            |?     |*     |1     |?     |0     |      |CB 6A |      |       |8       |Test bit b of register r.                                    |
|BIT 5,E                            |?     |*     |1     |?     |0     |      |CB 6B |      |       |8       |Test bit b of register r.                                    |
|BIT 5,H                            |?     |*     |1     |?     |0     |      |CB 6C |      |       |8       |Test bit b of register r.                                    |
|BIT 5,L                            |?     |*     |1     |?     |0     |      |CB 6D |      |       |8       |Test bit b of register r.                                    |
|BIT 6,(HL)                         |?     |*     |1     |?     |0     |      |CB 76 |      |       |12      |Test bit b of location (HL).                                 |
|BIT 6,(IX+n)                       |?     |*     |1     |?     |0     |      |DD CB |XX    |76     |20      |Test bit b of location (IX+N).                               |
|BIT 6,(IY+n)                       |?     |*     |1     |?     |0     |      |FD CB |XX    |76     |20      |Test bit b of location (IY+N).                               |
|BIT 6,A                            |?     |*     |1     |?     |0     |      |CB 77 |      |       |8       |Test bit b of register r.                                    |
|BIT 6,B                            |?     |*     |1     |?     |0     |      |CB 70 |      |       |8       |Test bit b of register r.                                    |
|BIT 6,C                            |?     |*     |1     |?     |0     |      |CB 71 |      |       |8       |Test bit b of register r.                                    |
|BIT 6,D                            |?     |*     |1     |?     |0     |      |CB 72 |      |       |8       |Test bit b of register r.                                    |
|BIT 6,E                            |?     |*     |1     |?     |0     |      |CB 73 |      |       |8       |Test bit b of register r.                                    |
|BIT 6,H                            |?     |*     |1     |?     |0     |      |CB 74 |      |       |8       |Test bit b of register r.                                    |
|BIT 6,L                            |?     |*     |1     |?     |0     |      |CB 75 |      |       |8       |Test bit b of register r.                                    |
|BIT 7,(HL)                         |?     |*     |1     |?     |0     |      |CB 7E |      |       |12      |Test bit b of location (HL).                                 |
|BIT 7,(IX+n)                       |?     |*     |1     |?     |0     |      |DD CB |XX    |7E     |20      |Test bit b of location (IX+N).                               |
|BIT 7,(IY+n)                       |?     |*     |1     |?     |0     |      |FD CB |XX    |7E     |20      |Test bit b of location (IY+N).                               |
|BIT 7,A                            |?     |*     |1     |?     |0     |      |CB 7F |      |       |8       |Test bit b of register r.                                    |
|BIT 7,B                            |?     |*     |1     |?     |0     |      |CB 78 |      |       |8       |Test bit b of register r.                                    |
|BIT 7,C                            |?     |*     |1     |?     |0     |      |CB 79 |      |       |8       |Test bit b of register r.                                    |
|BIT 7,D                            |?     |*     |1     |?     |0     |      |CB 7A |      |       |8       |Test bit b of register r.                                    |
|BIT 7,E                            |?     |*     |1     |?     |0     |      |CB 7B |      |       |8       |Test bit b of register r.                                    |
|BIT 7,H                            |?     |*     |1     |?     |0     |      |CB 7C |      |       |8       |Test bit b of register r.                                    |
|BIT 7,L                            |?     |*     |1     |?     |0     |      |CB 7D |      |       |8       |Test bit b of register r.                                    |
|CALL C,nn                          |      |      |      |      |      |      |DC    |XX XX |       |10      |Call subroutine at location nn if condition CC is true.      |
|CALL M,nn                          |      |      |      |      |      |      |FC    |XX XX |       |10      |Call subroutine at location nn if condition CC is true.      |
|CALL NC,nn                         |      |      |      |      |      |      |D4    |XX XX |       |10      |Call subroutine at location nn if condition CC is true.      |
|CALL nn                            |      |      |      |      |      |      |CD    |XX XX |       |17      |Call subroutine at location.                                 |
|CALL NZ,nn                         |      |      |      |      |      |      |C4    |XX XX |       |10      |Call subroutine at location nn if condition CC is true.      |
|CALL P,nn                          |      |      |      |      |      |      |F4    |XX XX |       |10      |Call subroutine at location nn if condition CC is true.      |
|CALL PE,nn                         |      |      |      |      |      |      |EC    |XX XX |       |10      |Call subroutine at location nn if condition CC is true.      |
|CALL PO,nn                         |      |      |      |      |      |      |E4    |XX XX |       |10      |Call subroutine at location nn if condition CC is true.      |
|CALL Z,nn                          |      |      |      |      |      |      |CC    |XX XX |       |10      |Call subroutine at location nn if condition CC is true.      |
|CCF                                |      |      |?     |      |0     |*     |3F    |      |       |4       |Complement carry flag.                                       |
|CP (HL)                            |*     |*     |*     |V     |1     |*     |BE    |      |       |7       |Compare value at location (HL) with accumulator.             |
|CP (IX+n)                          |*     |*     |*     |V     |1     |*     |DD BE |XX    |       |19      |Compare value at location (IX+N) with accumulator.           |
|CP (IY+n)                          |*     |*     |*     |V     |1     |*     |FD BE |XX    |       |19      |Compare value at location (IY+N) with accumulator.           |
|CP A                               |*     |*     |*     |V     |1     |*     |BF    |      |       |4       |Compare register r with accumulator.                         |
|CP B                               |*     |*     |*     |V     |1     |*     |B8    |      |       |4       |Compare register r with accumulator.                         |
|CP C                               |*     |*     |*     |V     |1     |*     |B9    |      |       |4       |Compare register r with accumulator.                         |
|CP D                               |*     |*     |*     |V     |1     |*     |BA    |      |       |4       |Compare register r with accumulator.                         |
|CP E                               |*     |*     |*     |V     |1     |*     |BB    |      |       |4       |Compare register r with accumulator.                         |
|CP H                               |*     |*     |*     |V     |1     |*     |BC    |      |       |4       |Compare register r with accumulator.                         |
|CP L                               |*     |*     |*     |V     |1     |*     |BD    |      |       |4       |Compare register r with accumulator.                         |
|CP n                               |*     |*     |*     |V     |1     |*     |FE    |XX    |       |7       |Compare value n with accumulator.                            |
|CPD                                |*     |*     |*     |*     |1     |      |ED A9 |      |       |21/16   |Compare location (HL) and acc., decrement HL and BC,         |
|CPDR                               |*     |*     |*     |*     |1     |      |ED B9 |      |       |16      |Perform a CPD and repeat until BC=0.                         |
|CPI                                |*     |*     |*     |*     |1     |      |ED A1 |      |       |16      |Compare location (HL) and acc., incr HL, decr BC.            |
|CPIR                               |*     |*     |*     |*     |1     |      |ED B1 |      |       |16      |Perform a CPI and repeat until BC=0.                         |
|CPL                                |      |      |1     |      |1     |      |2F    |      |       |4       |Complement accumulator (1's complement).                     |
|DAA                                |*     |*     |*     |P     |      |*     |27    |      |       |4       |Decimal adjust accumulator.                                  |
|DEC (HL)                           |*     |*     |*     |V     |1     |      |35    |      |       |11      |Decrement value at location (HL).                            |
|DEC (IX+n)                         |*     |*     |*     |V     |1     |      |DD 35 |XX    |       |23      |Decrement value at location (IX+N).                          |
|DEC (IY+n)                         |*     |*     |*     |V     |1     |      |FD 35 |XX    |       |23      |Decrement value at location (IY+N).                          |
|DEC A                              |*     |*     |*     |V     |1     |      |3D    |      |       |4       |Decrement register r.                                        |
|DEC B                              |*     |*     |*     |V     |1     |      |05    |      |       |4       |Decrement register r.                                        |
|DEC BC                             |      |      |      |      |      |      |0B    |      |       |6       |Decrement register pair BC.                                  |
|DEC C                              |*     |*     |*     |V     |1     |      |0D    |      |       |4       |Decrement register r.                                        |
|DEC D                              |*     |*     |*     |V     |1     |      |15    |      |       |4       |Decrement register r.                                        |
|DEC DE                             |      |      |      |      |      |      |1B    |      |       |6       |Decrement register pair DE.                                  |
|DEC E                              |*     |*     |*     |V     |1     |      |1D    |      |       |4       |Decrement register r.                                        |
|DEC H                              |*     |*     |*     |V     |1     |      |25    |      |       |4       |Decrement register r.                                        |
|DEC HL                             |      |      |      |      |      |      |2B    |      |       |6       |Decrement register pair HL.                                  |
|DEC IX                             |      |      |      |      |      |      |DD 2B |      |       |10      |Decrement IX.                                                |
|DEC IY                             |      |      |      |      |      |      |FD 2B |      |       |10      |Decrement IY.                                                |
|DEC L                              |*     |*     |*     |V     |1     |      |2D    |      |       |4       |Decrement register r.                                        |
|DEC SP                             |      |      |      |      |      |      |3B    |      |       |6       |Decrement register pair SP.                                  |
|DI                                 |      |      |      |      |      |      |F3    |      |       |4       |Disable interrupts. (except NMI at 0066h)                    |
|DJNZ n                             |      |      |      |      |      |      |10    |      |       |13/8    |Decrement B and jump relative if B<>0.                       |
|EI                                 |      |      |      |      |      |      |FB    |      |       |4       |Enable interrupts.                                           |
|EX (SP),HL                         |      |      |      |      |      |      |E3    |      |       |19      |Exchange the location (SP) and HL.                           |
|EX (SP),IX                         |      |      |      |      |      |      |DD E3 |      |       |23      |Exchange the location (SP) and IX.                           |
|EX (SP),IY                         |      |      |      |      |      |      |FD E3 |      |       |23      |Exchange the location (SP) and IY.                           |
|EX AF,AF'                          |      |      |      |      |      |      |08    |      |       |4       |Exchange the contents of AF and AF'.                         |
|EX DE,HL                           |      |      |      |      |      |      |EB    |      |       |4       |Exchange the contents of DE and HL.                          |
|EXX                                |      |      |      |      |      |      |D9    |      |       |4       |Exchange the contents of BC,DE,HL with BC',DE',HL'.          |
|HALT                               |      |      |      |      |      |      |76    |      |       |4       |Halt computer and wait for interrupt.                        |
|IM 0                               |      |      |      |      |      |      |ED 46 |      |       |8       |Set interrupt mode 0. (instruction on data bus by int device)|
|IM 1                               |      |      |      |      |      |      |ED 56 |      |       |8       |Set interrupt mode 1. (rst 38)                               |
|IM 2                               |      |      |      |      |      |      |ED 5E |      |       |8       |Set interrupt mode 2. (vector jump)                          |
|IN A,(C)                           |*     |*     |*     |P     |0     |      |ED 78 |      |       |12      |Load the register r with input from device (C).              |
|IN A,(n)                           |      |      |      |      |      |      |DB    |XX    |       |11      |Load the accumulator with input from device n.               |
|IN B,(C)                           |*     |*     |*     |P     |0     |      |ED 40 |      |       |12      |Load the register r with input from device (C).              |
|IN C,(C)                           |*     |*     |*     |P     |0     |      |ED 48 |      |       |12      |Load the register r with input from device (C).              |
|IN D,(C)                           |*     |*     |*     |P     |0     |      |ED 50 |      |       |12      |Load the register r with input from device (C).              |
|IN E,(C)                           |*     |*     |*     |P     |0     |      |ED 58 |      |       |12      |Load the register r with input from device (C).              |
|IN H,(C)                           |*     |*     |*     |P     |0     |      |ED 60 |      |       |12      |Load the register r with input from device (C).              |
|IN L,(C)                           |*     |*     |*     |P     |0     |      |ED 68 |      |       |12      |Load the register r with input from device (C).              |
|INC (HL)                           |*     |*     |*     |V     |0     |      |34    |      |       |11      |Increment location (HL).                                     |
|INC (IX+n)                         |*     |*     |*     |V     |0     |      |DD 34 |XX    |       |23      |Increment location (IX+n).                                   |
|INC (IY+n)                         |*     |*     |*     |V     |0     |      |FD 34 |XX    |       |23      |Increment location (IY+n).                                   |
|INC A                              |*     |*     |*     |V     |0     |      |3C    |      |       |4       |Increment register r.                                        |
|INC B                              |*     |*     |*     |V     |0     |      |04    |      |       |4       |Increment register r.                                        |
|INC BC                             |      |      |      |      |      |      |03    |      |       |6       |Increment register pair BC.                                  |
|INC C                              |*     |*     |*     |V     |0     |      |0C    |      |       |4       |Increment register r.                                        |
|INC D                              |*     |*     |*     |V     |0     |      |14    |      |       |4       |Increment register r.                                        |
|INC DE                             |      |      |      |      |      |      |13    |      |       |6       |Increment register pair DE.                                  |
|INC E                              |*     |*     |*     |V     |0     |      |1C    |      |       |4       |Increment register r.                                        |
|INC H                              |*     |*     |*     |V     |0     |      |24    |      |       |4       |Increment register r.                                        |
|INC HL                             |      |      |      |      |      |      |23    |      |       |6       |Increment register pair HL.                                  |
|INC IX                             |      |      |      |      |      |      |DD 23 |      |       |10      |Increment IX.                                                |
|INC IY                             |      |      |      |      |      |      |FD 23 |      |       |10      |Increment IY.                                                |
|INC L                              |*     |*     |*     |V     |0     |      |2C    |      |       |4       |Increment register r.                                        |
|INC SP                             |      |      |      |      |      |      |33    |      |       |6       |Increment register pair SP.                                  |
|IND                                |?     |*     |?     |?     |1     |      |ED AA |      |       |16      |(HL)=Input from port (C). Decrement HL and B.                |
|INDR                               |?     |1     |?     |?     |1     |      |ED BA |      |       |21/16   |Perform an IND and repeat until B=0.                         |
|INI                                |?     |*     |?     |?     |1     |      |ED A2 |      |       |16      |(HL)=Input from port (C). HL=HL+1. B=B-1.                    |
|INIR                               |?     |1     |?     |?     |1     |      |ED B2 |      |       |21/16   |Perform an INI and repeat until B=0.                         |
|JP (HL)                            |      |      |      |      |      |      |E9    |      |       |4       |Unconditional jump to location (HL).                         |
|JP (IX)                            |      |      |      |      |      |      |DD E9 |      |       |8       |Unconditional jump to location (IX).                         |
|JP (IY)                            |      |      |      |      |      |      |FD E9 |      |       |8       |Unconditional jump to location (IY).                         |
|JP C,nn                            |      |      |      |      |      |      |DA    |XX XX |       |10      |Jump to location nn if condition cc is true.                 |
|JP M,nn                            |      |      |      |      |      |      |FA    |XX XX |       |10      |Jump to location nn if condition cc is true.                 |
|JP NC,nn                           |      |      |      |      |      |      |D2    |XX XX |       |10      |Jump to location nn if condition cc is true.                 |
|JP nn                              |      |      |      |      |      |      |C3    |XX XX |       |10      |Unconditional jump to location nn                            |
|JP NZ,nn                           |      |      |      |      |      |      |C2    |XX XX |       |10      |Jump to location nn if condition cc is true.                 |
|JP P,nn                            |      |      |      |      |      |      |F2    |XX XX |       |10      |Jump to location nn if condition cc is true.                 |
|JP PE,nn                           |      |      |      |      |      |      |EA    |XX XX |       |10      |Jump to location nn if condition cc is true.                 |
|JP PO,nn                           |      |      |      |      |      |      |E2    |XX XX |       |10      |Jump to location nn if condition cc is true.                 |
|JP Z,nn                            |      |      |      |      |      |      |CA    |XX XX |       |10      |Jump to location nn if condition cc is true.                 |
|JR C,n                             |      |      |      |      |      |      |38    |XX    |       |10      |Jump to location nn if condition cc is true.                 |
|JR n                               |      |      |      |      |      |      |18    |XX    |       |12      |Unconditional jump relative to PC+n.                         |
|JR NC,n                            |      |      |      |      |      |      |30    |XX    |       |10      |Jump to location nn if condition cc is true.                 |
|JR NZ,n                            |      |      |      |      |      |      |20    |XX    |       |10      |Jump to location nn if condition cc is true.                 |
|JR Z,n                             |      |      |      |      |      |      |28    |XX    |       |10      |Jump to location nn if condition cc is true.                 |
|LD (BC),A                          |      |      |      |      |      |      |02    |      |       |7       |Load location (BC) with accumulator.                         |
|LD (DE),A                          |      |      |      |      |      |      |12    |      |       |7       |Load location (DE) with accumulator.                         |
|LD (HL),A                          |      |      |      |      |      |      |77    |      |       |7       |Load location (HL) with register r.                          |
|LD (HL),B                          |      |      |      |      |      |      |70    |      |       |7       |Load location (HL) with register r.                          |
|LD (HL),C                          |      |      |      |      |      |      |71    |      |       |7       |Load location (HL) with register r.                          |
|LD (HL),D                          |      |      |      |      |      |      |72    |      |       |7       |Load location (HL) with register r.                          |
|LD (HL),E                          |      |      |      |      |      |      |73    |      |       |7       |Load location (HL) with register r.                          |
|LD (HL),H                          |      |      |      |      |      |      |74    |      |       |7       |Load location (HL) with register r.                          |
|LD (HL),L                          |      |      |      |      |      |      |75    |      |       |7       |Load location (HL) with register r.                          |
|LD (HL),n                          |      |      |      |      |      |      |36    |XX    |       |10      |Load location (HL) with value n.                             |
|LD (IX+n),A                        |      |      |      |      |      |      |DD 77 |XX    |       |19      |Load location (IX+n) with register r.                        |
|LD (IX+n),B                        |      |      |      |      |      |      |DD 70 |XX    |       |19      |Load location (IX+n) with register r.                        |
|LD (IX+n),C                        |      |      |      |      |      |      |DD 71 |XX    |       |19      |Load location (IX+n) with register r.                        |
|LD (IX+n),D                        |      |      |      |      |      |      |DD 72 |XX    |       |19      |Load location (IX+n) with register r.                        |
|LD (IX+n),E                        |      |      |      |      |      |      |DD 73 |XX    |       |19      |Load location (IX+n) with register r.                        |
|LD (IX+n),H                        |      |      |      |      |      |      |DD 74 |XX    |       |19      |Load location (IX+n) with register r.                        |
|LD (IX+n),L                        |      |      |      |      |      |      |DD 75 |XX    |       |19      |Load location (IX+n) with register r.                        |
|LD (IX+n),n                        |      |      |      |      |      |      |DD 36 |XX XX |       |19      |Load location (IX+n) with value n.                           |
|LD (IY+n),A                        |      |      |      |      |      |      |FD 77 |XX    |       |19      |Load location (IY+n) with register r.                        |
|LD (IY+n),B                        |      |      |      |      |      |      |FD 70 |XX    |       |19      |Load location (IY+n) with register r.                        |
|LD (IY+n),C                        |      |      |      |      |      |      |FD 71 |XX    |       |19      |Load location (IY+n) with register r.                        |
|LD (IY+n),D                        |      |      |      |      |      |      |FD 72 |XX    |       |19      |Load location (IY+n) with register r.                        |
|LD (IY+n),E                        |      |      |      |      |      |      |FD 73 |XX    |       |19      |Load location (IY+n) with register r.                        |
|LD (IY+n),H                        |      |      |      |      |      |      |FD 74 |XX    |       |19      |Load location (IY+n) with register r.                        |
|LD (IY+n),L                        |      |      |      |      |      |      |FD 75 |XX    |       |19      |Load location (IY+n) with register r.                        |
|LD (IY+n),n                        |      |      |      |      |      |      |FD 36 |XX XX |       |19      |Load location (IY+n) with value n.                           |
|LD (nn),A                          |      |      |      |      |      |      |32    |XX XX |       |13      |Load location (nn) with accumulator.                         |
|LD (nn),BC                         |      |      |      |      |      |      |ED 43 |XX XX |       |20      |Load location (nn) with register pair BC.                    |
|LD (nn),DE                         |      |      |      |      |      |      |ED 53 |XX XX |       |20      |Load location (nn) with register pair DE.                    |
|LD (nn),HL                         |      |      |      |      |      |      |22    |XX XX |       |16      |Load location (nn) with HL.                                  |
|LD (nn),IX                         |      |      |      |      |      |      |DD 22 |XX XX |       |20      |Load location (nn) with IX.                                  |
|LD (nn),IY                         |      |      |      |      |      |      |FD 22 |XX XX |       |20      |Load location (nn) with IY.                                  |
|LD (nn),SP                         |      |      |      |      |      |      |ED 73 |XX XX |       |20      |Load location (nn) with register pair SP.                    |
|LD A,(BC)                          |*     |*     |0     |*     |0     |      |0A    |      |       |7       |Load accumulator with value at location (BC).                |
|LD A,(DE)                          |*     |*     |0     |*     |0     |      |1A    |      |       |7       |Load accumulator with value at location (DE).                |
|LD A,(HL)                          |*     |*     |0     |*     |0     |      |7E    |      |       |7       |Load accumulator with value at location (HL).                |
|LD A,(IX+n)                        |*     |*     |0     |*     |0     |      |DD 7E |XX    |       |19      |Load register r with value at location (IX+n).               |
|LD A,(IY+n)                        |*     |*     |0     |*     |0     |      |FD 7E |XX    |       |19      |Load register r with value at location (IY+n).               |
|LD A,(nn)                          |*     |*     |0     |*     |0     |      |3A    |XX XX |       |13      |Load accumulator with value at location nn.                  |
|LD A,A                             |*     |*     |0     |*     |0     |      |7F    |      |       |4       |Load register r with register r'.                            |
|LD A,B                             |*     |*     |0     |*     |0     |      |78    |      |       |4       |Load register r with register r'.                            |
|LD A,C                             |*     |*     |0     |*     |0     |      |79    |      |       |4       |Load register r with register r'.                            |
|LD A,D                             |*     |*     |0     |*     |0     |      |7A    |      |       |4       |Load register r with register r'.                            |
|LD A,E                             |*     |*     |0     |*     |0     |      |7B    |      |       |4       |Load register r with register r'.                            |
|LD A,H                             |*     |*     |0     |*     |0     |      |7C    |      |       |4       |Load register r with register r'.                            |
|LD A,I                             |*     |*     |0     |*     |0     |      |ED 57 |      |       |9       |Load accumulator with I.(interrupt vector register)          |
|LD A,L                             |*     |*     |0     |*     |0     |      |7D    |      |       |4       |Load register r with register r'.                            |
|LD A,n                             |*     |*     |0     |*     |0     |      |3E    |XX    |       |7       |Load register r with value n.                                |
|LD A,R                             |*     |*     |0     |*     |0     |      |ED 5F |      |       |9       |Load accumulator with R.(memory refresh register)            |
|LD B,(HL)                          |      |      |      |      |      |      |46    |      |       |7       |Load register r with value at location (HL).                 |
|LD B,(IX+n)                        |      |      |      |      |      |      |DD 46 |XX    |       |19      |Load register r with value at location (IX+n).               |
|LD B,(IY+n)                        |      |      |      |      |      |      |FD 46 |XX    |       |19      |Load register r with value at location (IY+n).               |
|LD B,A                             |      |      |      |      |      |      |47    |      |       |4       |Load register r with register r'.                            |
|LD B,B                             |      |      |      |      |      |      |40    |      |       |4       |Load register r with register r'.                            |
|LD B,C                             |      |      |      |      |      |      |41    |      |       |4       |Load register r with register r'.                            |
|LD B,D                             |      |      |      |      |      |      |42    |      |       |4       |Load register r with register r'.                            |
|LD B,E                             |      |      |      |      |      |      |43    |      |       |4       |Load register r with register r'.                            |
|LD B,H                             |      |      |      |      |      |      |44    |      |       |4       |Load register r with register r'.                            |
|LD B,L                             |      |      |      |      |      |      |45    |      |       |4       |Load register r with register r'.                            |
|LD B,n                             |      |      |      |      |      |      |06    |XX    |       |7       |Load register r with value n.                                |
|LD BC,(nn)                         |      |      |      |      |      |      |ED 4B |XX XX |       |20      |Load register pair BC with value at location (nn).           |
|LD BC,nn                           |      |      |      |      |      |      |01    |XX XX |       |10      |Load register pair BC with nn.                               |
|LD C,(HL)                          |      |      |      |      |      |      |4E    |      |       |7       |Load register r with value at location (HL).                 |
|LD C,(IX+n)                        |      |      |      |      |      |      |DD 4E |XX    |       |19      |Load register r with value at location (IX+n).               |
|LD C,(IY+n)                        |      |      |      |      |      |      |FD 4E |XX    |       |19      |Load register r with value at location (IY+n).               |
|LD C,A                             |      |      |      |      |      |      |4F    |      |       |4       |Load register r with register r'.                            |
|LD C,B                             |      |      |      |      |      |      |48    |      |       |4       |Load register r with register r'.                            |
|LD C,C                             |      |      |      |      |      |      |49    |      |       |4       |Load register r with register r'.                            |
|LD C,D                             |      |      |      |      |      |      |4A    |      |       |4       |Load register r with register r'.                            |
|LD C,E                             |      |      |      |      |      |      |4B    |      |       |4       |Load register r with register r'.                            |
|LD C,H                             |      |      |      |      |      |      |4C    |      |       |4       |Load register r with register r'.                            |
|LD C,L                             |      |      |      |      |      |      |4D    |      |       |4       |Load register r with register r'.                            |
|LD C,n                             |      |      |      |      |      |      |0E    |XX    |       |7       |Load register r with value n.                                |
|LD D,(HL)                          |      |      |      |      |      |      |56    |      |       |7       |Load register r with value at location (HL).                 |
|LD D,(IX+n)                        |      |      |      |      |      |      |DD 56 |XX    |       |19      |Load register r with value at location (IX+n).               |
|LD D,(IY+n)                        |      |      |      |      |      |      |FD 56 |XX    |       |19      |Load register r with value at location (IY+n).               |
|LD D,A                             |      |      |      |      |      |      |57    |      |       |4       |Load register r with register r'.                            |
|LD D,B                             |      |      |      |      |      |      |50    |      |       |4       |Load register r with register r'.                            |
|LD D,C                             |      |      |      |      |      |      |51    |      |       |4       |Load register r with register r'.                            |
|LD D,D                             |      |      |      |      |      |      |52    |      |       |4       |Load register r with register r'.                            |
|LD D,E                             |      |      |      |      |      |      |53    |      |       |4       |Load register r with register r'.                            |
|LD D,H                             |      |      |      |      |      |      |54    |      |       |4       |Load register r with register r'.                            |
|LD D,L                             |      |      |      |      |      |      |55    |      |       |4       |Load register r with register r'.                            |
|LD D,n                             |      |      |      |      |      |      |16    |XX    |       |7       |Load register r with value n.                                |
|LD DE,(nn)                         |      |      |      |      |      |      |ED 5B |XX XX |       |20      |Load register pair DE with value at location (nn).           |
|LD DE,nn                           |      |      |      |      |      |      |11    |XX XX |       |10      |Load register pair DE with nn.                               |
|LD E,(HL)                          |      |      |      |      |      |      |5E    |      |       |7       |Load register r with value at location (HL).                 |
|LD E,(IX+n)                        |      |      |      |      |      |      |DD 5E |XX    |       |19      |Load register r with value at location (IX+n).               |
|LD E,(IY+n)                        |      |      |      |      |      |      |FD 5E |XX    |       |19      |Load register r with value at location (IY+n).               |
|LD E,A                             |      |      |      |      |      |      |5F    |      |       |4       |Load register r with register r'.                            |
|LD E,B                             |      |      |      |      |      |      |58    |      |       |4       |Load register r with register r'.                            |
|LD E,C                             |      |      |      |      |      |      |59    |      |       |4       |Load register r with register r'.                            |
|LD E,D                             |      |      |      |      |      |      |5A    |      |       |4       |Load register r with register r'.                            |
|LD E,E                             |      |      |      |      |      |      |5B    |      |       |4       |Load register r with register r'.                            |
|LD E,H                             |      |      |      |      |      |      |5C    |      |       |4       |Load register r with register r'.                            |
|LD E,L                             |      |      |      |      |      |      |5D    |      |       |4       |Load register r with register r'.                            |
|LD E,n                             |      |      |      |      |      |      |1E    |XX    |       |7       |Load register r with value n.                                |
|LD H,(HL)                          |      |      |      |      |      |      |66    |      |       |7       |Load register r with value at location (HL).                 |
|LD H,(IX+n)                        |      |      |      |      |      |      |DD 66 |XX    |       |19      |Load register r with value at location (IX+n).               |
|LD H,(IY+n)                        |      |      |      |      |      |      |FD 66 |XX    |       |19      |Load register r with value at location (IY+n).               |
|LD H,A                             |      |      |      |      |      |      |67    |      |       |4       |Load register r with register r'.                            |
|LD H,B                             |      |      |      |      |      |      |60    |      |       |4       |Load register r with register r'.                            |
|LD H,C                             |      |      |      |      |      |      |61    |      |       |4       |Load register r with register r'.                            |
|LD H,D                             |      |      |      |      |      |      |62    |      |       |4       |Load register r with register r'.                            |
|LD H,E                             |      |      |      |      |      |      |63    |      |       |4       |Load register r with register r'.                            |
|LD H,H                             |      |      |      |      |      |      |64    |      |       |4       |Load register r with register r'.                            |
|LD H,L                             |      |      |      |      |      |      |65    |      |       |4       |Load register r with register r'.                            |
|LD H,n                             |      |      |      |      |      |      |26    |XX    |       |7       |Load register r with value n.                                |
|LD HL,(nn)                         |      |      |      |      |      |      |2A    |XX XX |       |16      |Load HL with value at location (nn). (L-first)               |
|LD HL,nn                           |      |      |      |      |      |      |21    |XX XX |       |10      |Load register pair HL with nn.                               |
|LD I,A                             |      |      |      |      |      |      |ED 47 |      |       |9       |Load I with accumulator.                                     |
|LD IX,(nn)                         |      |      |      |      |      |      |DD 2A |XX XX |       |20      |Load IX with value at location (nn).                         |
|LD IX,nn                           |      |      |      |      |      |      |DD 21 |XX XX |       |14      |Load IX with value nn.                                       |
|LD IY,(nn)                         |      |      |      |      |      |      |FD 2A |XX XX |       |20      |Load IY with value at location (nn).                         |
|LD IY,nn                           |      |      |      |      |      |      |FD 21 |XX XX |       |14      |Load IY with value nn.                                       |
|LD L,(HL)                          |      |      |      |      |      |      |6E    |      |       |7       |Load register r with value at location (HL).                 |
|LD L,(IX+n)                        |      |      |      |      |      |      |DD 6E |XX    |       |19      |Load register r with value at location (IX+n).               |
|LD L,(IY+n)                        |      |      |      |      |      |      |FD 6E |XX    |       |19      |Load register r with value at location (IY+n).               |
|LD L,A                             |      |      |      |      |      |      |6F    |      |       |4       |Load register r with register r'.                            |
|LD L,B                             |      |      |      |      |      |      |68    |      |       |4       |Load register r with register r'.                            |
|LD L,C                             |      |      |      |      |      |      |69    |      |       |4       |Load register r with register r'.                            |
|LD L,D                             |      |      |      |      |      |      |6A    |      |       |4       |Load register r with register r'.                            |
|LD L,E                             |      |      |      |      |      |      |6B    |      |       |4       |Load register r with register r'.                            |
|LD L,H                             |      |      |      |      |      |      |6C    |      |       |4       |Load register r with register r'.                            |
|LD L,L                             |      |      |      |      |      |      |6D    |      |       |4       |Load register r with register r'.                            |
|LD L,n                             |      |      |      |      |      |      |2E    |XX    |       |7       |Load register r with value n.                                |
|LD SP,(nn)                         |      |      |      |      |      |      |ED 7B |XX XX |       |20      |Load register pair SP with value at location (nn).           |
|LD SP,HL                           |      |      |      |      |      |      |F9    |      |       |6       |Load SP with HL.                                             |
|LD SP,IX                           |      |      |      |      |      |      |DD F9 |      |       |10      |Load SP with IX.                                             |
|LD SP,IY                           |      |      |      |      |      |      |FD F9 |      |       |10      |Load SP with IY.                                             |
|LD SP,nn                           |      |      |      |      |      |      |31    |XX XX |       |10      |Load register pair SP with nn.                               |
|LDD                                |      |      |0     |0     |0     |      |ED A8 |      |       |16      |Load location (DE) with location (HL), decrement DE,HL,BC.   |
|LDDR                               |      |      |0     |*     |0     |      |ED B8 |      |       |21/16   |Perform an LDD and repeat until BC=0.                        |
|LDI                                |      |      |0     |0     |0     |      |ED A0 |      |       |16      |Load location (DE) with location (HL), incr DE,HL; decr BC.  |
|LDIR                               |      |      |      |      |      |      |ED B0 |      |       |21/16   |Perform an LDI and repeat until BC=0.                        |
|NEG                                |*     |*     |*     |V     |1     |*     |ED 44 |      |       |8       |Negate accumulator (2's complement).                         |
|NOP                                |      |      |      |      |      |      |00    |      |       |4       |No operation.                                                |
|OR (HL)                            |*     |*     |*     |P     |0     |0     |B6    |      |       |7       |Logical OR of value at location (HL) and accumulator.        |
|OR (IX+n)                          |*     |*     |*     |P     |0     |0     |DD B6 |XX    |       |19      |Logical OR of value at location (IX+N) and accumulator.      |
|OR (IY+n)                          |*     |*     |*     |P     |0     |0     |FD B6 |XX    |       |19      |Logical OR of value at location (IY+N) and accumulator.      |
|OR A                               |*     |*     |*     |P     |0     |0     |B7    |      |       |4       |Logical OR of register r and accumulator.                    |
|OR B                               |*     |*     |*     |P     |0     |0     |B0    |      |       |4       |Logical OR of register r and accumulator.                    |
|OR C                               |*     |*     |*     |P     |0     |0     |B1    |      |       |4       |Logical OR of register r and accumulator.                    |
|OR D                               |*     |*     |*     |P     |0     |0     |B2    |      |       |4       |Logical OR of register r and accumulator.                    |
|OR E                               |*     |*     |*     |P     |0     |0     |B3    |      |       |4       |Logical OR of register r and accumulator.                    |
|OR H                               |*     |*     |*     |P     |0     |0     |B4    |      |       |4       |Logical OR of register r and accumulator.                    |
|OR L                               |*     |*     |*     |P     |0     |0     |B5    |      |       |4       |Logical OR of register r and accumulator.                    |
|OR N                               |*     |*     |*     |P     |0     |0     |F6    |XX    |       |7       |Logical OR of value n and accumulator.                       |
|OTDR                               |?     |1     |?     |?     |?     |1     |ED BB |      |       |21/16   |Perform an OUTD and repeat until B=0.                        |
|OTIR                               |?     |1     |?     |?     |?     |1     |ED B3 |      |       |21/16   |Perform an OTI and repeat until B=0.                         |
|OUT (C),A                          |      |      |      |      |      |      |ED 79 |      |       |12      |Load output port (C) with register r.                        |
|OUT (C),B                          |      |      |      |      |      |      |ED 41 |      |       |12      |Load output port (C) with register r.                        |
|OUT (C),C                          |      |      |      |      |      |      |ED 49 |      |       |12      |Load output port (C) with register r.                        |
|OUT (C),D                          |      |      |      |      |      |      |ED 51 |      |       |12      |Load output port (C) with register r.                        |
|OUT (C),E                          |      |      |      |      |      |      |ED 59 |      |       |12      |Load output port (C) with register r.                        |
|OUT (C),H                          |      |      |      |      |      |      |ED 61 |      |       |12      |Load output port (C) with register r.                        |
|OUT (C),L                          |      |      |      |      |      |      |ED 69 |      |       |12      |Load output port (C) with register r.                        |
|OUT (N),A                          |      |      |      |      |      |      |D3    |XX    |       |11      |Load output port (n) with accumulator.                       |
|OUTD                               |?     |*     |?     |?     |1     |      |ED AB |      |       |16      |Load output port (C) with (HL), decrement HL and B.          |
|OUTI                               |?     |*     |?     |?     |1     |      |ED A3 |      |       |16      |Load output port (C) with (HL), incr HL, decr B.             |
|POP AF                             |      |      |      |      |      |      |F1    |      |       |10      |Load register pair AF with top of stack.                     |
|POP BC                             |      |      |      |      |      |      |C1    |      |       |10      |Load register pair BC with top of stack.                     |
|POP DE                             |      |      |      |      |      |      |D1    |      |       |10      |Load register pair DE with top of stack.                     |
|POP HL                             |      |      |      |      |      |      |E1    |      |       |10      |Load register pair HL with top of stack.                     |
|POP IX                             |      |      |      |      |      |      |DD E1 |      |       |14      |Load IX with top of stack.                                   |
|POP IY                             |      |      |      |      |      |      |FD E1 |      |       |14      |Load IY with top of stack.                                   |
|PUSH AF                            |      |      |      |      |      |      |F5    |      |       |11      |Load register pair AF onto stack.                            |
|PUSH BC                            |      |      |      |      |      |      |C5    |      |       |11      |Load register pair BC onto stack.                            |
|PUSH DE                            |      |      |      |      |      |      |D5    |      |       |11      |Load register pair DE onto stack.                            |
|PUSH HL                            |      |      |      |      |      |      |E5    |      |       |11      |Load register pair HL onto stack.                            |
|PUSH IX                            |      |      |      |      |      |      |DD E5 |      |       |15      |Load IX onto stack.                                          |
|PUSH IY                            |      |      |      |      |      |      |FD E5 |      |       |15      |Load IY onto stack.                                          |
|RES 0,(HL)                         |      |      |      |      |      |      |CB 86 |      |       |15      |Reset bit b in value at location (HL).                       |
|RES 0,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |86     |23      |Reset bit b in value at location (IX+N).                     |
|RES 0,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |86     |23      |Reset bit b in value at location (IY+N).                     |
|RES 0,A                            |      |      |      |      |      |      |CB 87 |      |       |8       |Reset bit b of register r.                                   |
|RES 0,B                            |      |      |      |      |      |      |CB 80 |      |       |8       |Reset bit b of register r.                                   |
|RES 0,C                            |      |      |      |      |      |      |CB 81 |      |       |8       |Reset bit b of register r.                                   |
|RES 0,D                            |      |      |      |      |      |      |CB 82 |      |       |8       |Reset bit b of register r.                                   |
|RES 0,E                            |      |      |      |      |      |      |CB 83 |      |       |8       |Reset bit b of register r.                                   |
|RES 0,H                            |      |      |      |      |      |      |CB 84 |      |       |8       |Reset bit b of register r.                                   |
|RES 0,L                            |      |      |      |      |      |      |CB 85 |      |       |8       |Reset bit b of register r.                                   |
|RES 1,(HL)                         |      |      |      |      |      |      |CB 8E |      |       |15      |Reset bit b in value at location (HL).                       |
|RES 1,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |8E     |23      |Reset bit b in value at location (IX+N).                     |
|RES 1,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |8E     |23      |Reset bit b in value at location (IY+N).                     |
|RES 1,A                            |      |      |      |      |      |      |CB 8F |      |       |8       |Reset bit b of register r.                                   |
|RES 1,B                            |      |      |      |      |      |      |CB 88 |      |       |8       |Reset bit b of register r.                                   |
|RES 1,C                            |      |      |      |      |      |      |CB 89 |      |       |8       |Reset bit b of register r.                                   |
|RES 1,D                            |      |      |      |      |      |      |CB 8A |      |       |8       |Reset bit b of register r.                                   |
|RES 1,E                            |      |      |      |      |      |      |CB 8B |      |       |8       |Reset bit b of register r.                                   |
|RES 1,H                            |      |      |      |      |      |      |CB 8C |      |       |8       |Reset bit b of register r.                                   |
|RES 1,L                            |      |      |      |      |      |      |CB 8D |      |       |8       |Reset bit b of register r.                                   |
|RES 2,(HL)                         |      |      |      |      |      |      |CB 96 |      |       |15      |Reset bit b in value at location (HL).                       |
|RES 2,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |96     |23      |Reset bit b in value at location (IX+N).                     |
|RES 2,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |96     |23      |Reset bit b in value at location (IY+N).                     |
|RES 2,A                            |      |      |      |      |      |      |CB 97 |      |       |8       |Reset bit b of register r.                                   |
|RES 2,B                            |      |      |      |      |      |      |CB 90 |      |       |8       |Reset bit b of register r.                                   |
|RES 2,C                            |      |      |      |      |      |      |CB 91 |      |       |8       |Reset bit b of register r.                                   |
|RES 2,D                            |      |      |      |      |      |      |CB 92 |      |       |8       |Reset bit b of register r.                                   |
|RES 2,E                            |      |      |      |      |      |      |CB 93 |      |       |8       |Reset bit b of register r.                                   |
|RES 2,H                            |      |      |      |      |      |      |CB 94 |      |       |8       |Reset bit b of register r.                                   |
|RES 2,L                            |      |      |      |      |      |      |CB 95 |      |       |8       |Reset bit b of register r.                                   |
|RES 3,(HL)                         |      |      |      |      |      |      |CB 9E |      |       |15      |Reset bit b in value at location (HL).                       |
|RES 3,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |9E     |23      |Reset bit b in value at location (IX+N).                     |
|RES 3,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |9E     |23      |Reset bit b in value at location (IY+N).                     |
|RES 3,A                            |      |      |      |      |      |      |CB 9F |      |       |8       |Reset bit b of register r.                                   |
|RES 3,B                            |      |      |      |      |      |      |CB 98 |      |       |8       |Reset bit b of register r.                                   |
|RES 3,C                            |      |      |      |      |      |      |CB 99 |      |       |8       |Reset bit b of register r.                                   |
|RES 3,D                            |      |      |      |      |      |      |CB 9A |      |       |8       |Reset bit b of register r.                                   |
|RES 3,E                            |      |      |      |      |      |      |CB 9B |      |       |8       |Reset bit b of register r.                                   |
|RES 3,H                            |      |      |      |      |      |      |CB 9C |      |       |8       |Reset bit b of register r.                                   |
|RES 3,L                            |      |      |      |      |      |      |CB 9D |      |       |8       |Reset bit b of register r.                                   |
|RES 4,(HL)                         |      |      |      |      |      |      |CB A6 |      |       |15      |Reset bit b in value at location (HL).                       |
|RES 4,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |A6     |23      |Reset bit b in value at location (IX+N).                     |
|RES 4,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |A6     |23      |Reset bit b in value at location (IY+N).                     |
|RES 4,A                            |      |      |      |      |      |      |CB A7 |      |       |8       |Reset bit b of register r.                                   |
|RES 4,B                            |      |      |      |      |      |      |CB A0 |      |       |8       |Reset bit b of register r.                                   |
|RES 4,C                            |      |      |      |      |      |      |CB A1 |      |       |8       |Reset bit b of register r.                                   |
|RES 4,D                            |      |      |      |      |      |      |CB A2 |      |       |8       |Reset bit b of register r.                                   |
|RES 4,E                            |      |      |      |      |      |      |CB A3 |      |       |8       |Reset bit b of register r.                                   |
|RES 4,H                            |      |      |      |      |      |      |CB A4 |      |       |8       |Reset bit b of register r.                                   |
|RES 4,L                            |      |      |      |      |      |      |CB A5 |      |       |8       |Reset bit b of register r.                                   |
|RES 5,(HL)                         |      |      |      |      |      |      |CB AE |      |       |15      |Reset bit b in value at location (HL).                       |
|RES 5,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |AE     |23      |Reset bit b in value at location (IX+N).                     |
|RES 5,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |AE     |23      |Reset bit b in value at location (IY+N).                     |
|RES 5,A                            |      |      |      |      |      |      |CB AF |      |       |8       |Reset bit b of register r.                                   |
|RES 5,B                            |      |      |      |      |      |      |CB A8 |      |       |8       |Reset bit b of register r.                                   |
|RES 5,C                            |      |      |      |      |      |      |CB A9 |      |       |8       |Reset bit b of register r.                                   |
|RES 5,D                            |      |      |      |      |      |      |CB AA |      |       |8       |Reset bit b of register r.                                   |
|RES 5,E                            |      |      |      |      |      |      |CB AB |      |       |8       |Reset bit b of register r.                                   |
|RES 5,H                            |      |      |      |      |      |      |CB AC |      |       |8       |Reset bit b of register r.                                   |
|RES 5,L                            |      |      |      |      |      |      |CB AD |      |       |8       |Reset bit b of register r.                                   |
|RES 6,(HL)                         |      |      |      |      |      |      |CB B6 |      |       |15      |Reset bit b in value at location (HL).                       |
|RES 6,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |B6     |23      |Reset bit b in value at location (IX+N).                     |
|RES 6,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |B6     |23      |Reset bit b in value at location (IY+N).                     |
|RES 6,A                            |      |      |      |      |      |      |CB B7 |      |       |8       |Reset bit b of register r.                                   |
|RES 6,B                            |      |      |      |      |      |      |CB B0 |      |       |8       |Reset bit b of register r.                                   |
|RES 6,C                            |      |      |      |      |      |      |CB B1 |      |       |8       |Reset bit b of register r.                                   |
|RES 6,D                            |      |      |      |      |      |      |CB B2 |      |       |8       |Reset bit b of register r.                                   |
|RES 6,E                            |      |      |      |      |      |      |CB B3 |      |       |8       |Reset bit b of register r.                                   |
|RES 6,H                            |      |      |      |      |      |      |CB B4 |      |       |8       |Reset bit b of register r.                                   |
|RES 6,L                            |      |      |      |      |      |      |CB B5 |      |       |8       |Reset bit b of register r.                                   |
|RES 7,(HL)                         |      |      |      |      |      |      |CB BE |      |       |15      |Reset bit b in value at location (HL).                       |
|RES 7,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |BE     |23      |Reset bit b in value at location (IX+N).                     |
|RES 7,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |BE     |23      |Reset bit b in value at location (IY+N).                     |
|RES 7,A                            |      |      |      |      |      |      |CB BF |      |       |8       |Reset bit b of register r.                                   |
|RES 7,B                            |      |      |      |      |      |      |CB B8 |      |       |8       |Reset bit b of register r.                                   |
|RES 7,C                            |      |      |      |      |      |      |CB B9 |      |       |8       |Reset bit b of register r.                                   |
|RES 7,D                            |      |      |      |      |      |      |CB BA |      |       |8       |Reset bit b of register r.                                   |
|RES 7,E                            |      |      |      |      |      |      |CB BB |      |       |8       |Reset bit b of register r.                                   |
|RES 7,H                            |      |      |      |      |      |      |CB BC |      |       |8       |Reset bit b of register r.                                   |
|RES 7,L                            |      |      |      |      |      |      |CB BD |      |       |8       |Reset bit b of register r.                                   |
|RET                                |      |      |      |      |      |      |C9    |      |       |10      |Return from subroutine.                                      |
|RET C                              |      |      |      |      |      |      |D8    |      |       |11/5    |Return from subroutine if condition cc is true.              |
|RET M                              |      |      |      |      |      |      |F8    |      |       |11/5    |Return from subroutine if condition cc is true.              |
|RET NC                             |      |      |      |      |      |      |D0    |      |       |11/5    |Return from subroutine if condition cc is true.              |
|RET NZ                             |      |      |      |      |      |      |C0    |      |       |11/5    |Return from subroutine if condition cc is true.              |
|RET P                              |      |      |      |      |      |      |F0    |      |       |11/5    |Return from subroutine if condition cc is true.              |
|RET PE                             |      |      |      |      |      |      |E8    |      |       |11/5    |Return from subroutine if condition cc is true.              |
|RET PO                             |      |      |      |      |      |      |E0    |      |       |11/5    |Return from subroutine if condition cc is true.              |
|RET Z                              |      |      |      |      |      |      |C8    |      |       |11/5    |Return from subroutine if condition cc is true.              |
|RETI                               |      |      |      |      |      |      |ED 4D |      |       |14      |Return from interrupt.                                       |
|RETN                               |      |      |      |      |      |      |ED 45 |      |       |14      |Return from non-maskable interrupt.                          |
|RL (HL)                            |*     |*     |0     |P     |0     |*     |CB 16 |      |       |15      |Rotate left through value at location (HL).                  |
|RL (IX+n)                          |*     |*     |0     |P     |0     |*     |DD CB |XX    |16     |23      |Rotate left through value at location (IX+N).                |
|RL (IY+n)                          |*     |*     |0     |P     |0     |*     |FD CB |XX    |16     |23      |Rotate left through value at location (IY+N).                |
|RL A                               |*     |*     |0     |P     |0     |*     |CB 17 |      |       |8       |Rotate left through register r.                              |
|RL B                               |*     |*     |0     |P     |0     |*     |CB 10 |      |       |8       |Rotate left through register r.                              |
|RL C                               |*     |*     |0     |P     |0     |*     |CB 11 |      |       |8       |Rotate left through register r.                              |
|RL D                               |*     |*     |0     |P     |0     |*     |CB 12 |      |       |8       |Rotate left through register r.                              |
|RL E                               |*     |*     |0     |P     |0     |*     |CB 13 |      |       |8       |Rotate left through register r.                              |
|RL H                               |*     |*     |0     |P     |0     |*     |CB 14 |      |       |8       |Rotate left through register r.                              |
|RL L                               |*     |*     |0     |P     |0     |*     |CB 15 |      |       |8       |Rotate left through register r.                              |
|RLA                                |      |      |0     |      |0     |*     |17    |      |       |4       |Rotate left accumulator through carry.                       |
|RLC (HL)                           |*     |*     |0     |P     |0     |*     |CB 06 |      |       |15      |Rotate location (HL) left circular.                          |
|RLC (IX+n)                         |*     |*     |0     |P     |0     |*     |DD CB |XX    |06     |23      |Rotate location (IX+N) left circular.                        |
|RLC (IY+n)                         |*     |*     |0     |P     |0     |*     |FD CB |XX    |06     |23      |Rotate location (IY+N) left circular.                        |
|RLC A                              |*     |*     |0     |P     |0     |*     |CB 07 |      |       |8       |Rotate register r left circular.                             |
|RLC B                              |*     |*     |0     |P     |0     |*     |CB 00 |      |       |8       |Rotate register r left circular.                             |
|RLC C                              |*     |*     |0     |P     |0     |*     |CB 01 |      |       |8       |Rotate register r left circular.                             |
|RLC D                              |*     |*     |0     |P     |0     |*     |CB 02 |      |       |8       |Rotate register r left circular.                             |
|RLC E                              |*     |*     |0     |P     |0     |*     |CB 03 |      |       |8       |Rotate register r left circular.                             |
|RLC H                              |*     |*     |0     |P     |0     |*     |CB 04 |      |       |8       |Rotate register r left circular.                             |
|RLC L                              |*     |*     |0     |P     |0     |*     |CB 05 |      |       |8       |Rotate register r left circular.                             |
|RLCA                               |      |      |0     |      |0     |*     |07    |      |       |4       |Rotate left circular accumulator.                            |
|RLD                                |*     |*     |0     |P     |0     |      |ED 6F |      |       |18      |Rotate digit left and right between accumulator and (HL).    |
|RR (HL)                            |*     |*     |0     |P     |0     |*     |CB 1E |      |       |15      |Rotate right through carry location (HL).                    |
|RR (IX+n)                          |*     |*     |0     |P     |0     |*     |DD CB |XX    |1E     |23      |Rotate right through carry location (IX+N).                  |
|RR (IY+n)                          |*     |*     |0     |P     |0     |*     |FD CB |XX    |1E     |23      |Rotate right through carry location (IY+N).                  |
|RR A                               |*     |*     |0     |P     |0     |*     |CB 1F |      |       |8       |Rotate right through carry register r.                       |
|RR B                               |*     |*     |0     |P     |0     |*     |CB 18 |      |       |8       |Rotate right through carry register r.                       |
|RR C                               |*     |*     |0     |P     |0     |*     |CB 19 |      |       |8       |Rotate right through carry register r.                       |
|RR D                               |*     |*     |0     |P     |0     |*     |CB 1A |      |       |8       |Rotate right through carry register r.                       |
|RR E                               |*     |*     |0     |P     |0     |*     |CB 1B |      |       |8       |Rotate right through carry register r.                       |
|RR H                               |*     |*     |0     |P     |0     |*     |CB 1C |      |       |8       |Rotate right through carry register r.                       |
|RR L                               |*     |*     |0     |P     |0     |*     |CB 1D |      |       |8       |Rotate right through carry register r.                       |
|RRA                                |      |      |0     |      |0     |*     |1F    |      |       |4       |Rotate right accumulator through carry.                      |
|RRC (HL)                           |*     |*     |0     |P     |0     |*     |CB 0E |      |       |15      |Rotate value at location (HL) right circular.                |
|RRC (IX+n)                         |*     |*     |0     |P     |0     |*     |DD CB |XX    |0E     |23      |Rotate value at location (IX+N) right circular.              |
|RRC (IY+n)                         |*     |*     |0     |P     |0     |*     |FD CB |XX    |0E     |23      |Rotate value at location (HL+N) right circular.              |
|RRC A                              |*     |*     |0     |P     |0     |*     |CB 0F |      |       |8       |Rotate register r right circular.                            |
|RRC B                              |*     |*     |0     |P     |0     |*     |CB 08 |      |       |8       |Rotate register r right circular.                            |
|RRC C                              |*     |*     |0     |P     |0     |*     |CB 09 |      |       |8       |Rotate register r right circular.                            |
|RRC D                              |*     |*     |0     |P     |0     |*     |CB 0A |      |       |8       |Rotate register r right circular.                            |
|RRC E                              |*     |*     |0     |P     |0     |*     |CB 0B |      |       |8       |Rotate register r right circular.                            |
|RRC H                              |*     |*     |0     |P     |0     |*     |CB 0C |      |       |8       |Rotate register r right circular.                            |
|RRC L                              |*     |*     |0     |P     |0     |*     |CB 0D |      |       |8       |Rotate register r right circular.                            |
|RRCA                               |      |      |0     |      |0     |*     |0F    |      |       |4       |Rotate right circular accumulator.                           |
|RRD                                |*     |*     |0     |P     |0     |      |ED 67 |      |       |18      |Rotate digit right and left between accumulator and (HL).    |
|RST 00H                            |      |      |      |      |      |      |C7    |      |       |11      |Restart to location 0000h.                                   |
|RST 08H                            |      |      |      |      |      |      |CF    |      |       |11      |Restart to location 0008h.                                   |
|RST 10H                            |      |      |      |      |      |      |D7    |      |       |11      |Restart to location 0010h.                                   |
|RST 18H                            |      |      |      |      |      |      |DF    |      |       |11      |Restart to location 0018h.                                   |
|RST 20H                            |      |      |      |      |      |      |E7    |      |       |11      |Restart to location 0020h.                                   |
|RST 28H                            |      |      |      |      |      |      |EF    |      |       |11      |Restart to location 0028h.                                   |
|RST 30H                            |      |      |      |      |      |      |F7    |      |       |11      |Restart to location 0030h.                                   |
|RST 38H                            |      |      |      |      |      |      |FF    |      |       |11      |Restart to location 0038h.                                   |
|SBC A                              |*     |*     |*     |V     |1     |*     |9F    |      |       |4       |Subtract register r from accumulator with carry.             |
|SBC A,(HL)                         |*     |*     |*     |V     |1     |*     |9E    |      |       |7       |Subtract value at location (HL) from accu. with carry.       |
|SBC A,(IX+n)                       |*     |*     |*     |V     |1     |*     |DD 9E |XX    |       |19      |Subtract value at location (IX+N) from accu. with carry.     |
|SBC A,(IY+n)                       |*     |*     |*     |V     |1     |*     |FD 9E |XX    |       |19      |Subtract value at location (IY+N) from accu. with carry.     |
|SBC A,n                            |*     |*     |*     |V     |1     |*     |DE    |XX    |       |7       |Subtract value n from accumulator with carry.                |
|SBC B                              |*     |*     |*     |V     |1     |*     |98    |      |       |4       |Subtract register r from accumulator with carry.             |
|SBC C                              |*     |*     |*     |V     |1     |*     |99    |      |       |4       |Subtract register r from accumulator with carry.             |
|SBC D                              |*     |*     |*     |V     |1     |*     |9A    |      |       |4       |Subtract register r from accumulator with carry.             |
|SBC E                              |*     |*     |*     |V     |1     |*     |9B    |      |       |4       |Subtract register r from accumulator with carry.             |
|SBC H                              |*     |*     |*     |V     |1     |*     |9C    |      |       |4       |Subtract register r from accumulator with carry.             |
|SBC HL,BC                          |*     |*     |?     |V     |1     |*     |ED 42 |      |       |15      |Subtract register pair BC from HL with carry.                |
|SBC HL,DE                          |*     |*     |?     |V     |1     |*     |ED 52 |      |       |15      |Subtract register pair DE from HL with carry.                |
|SBC HL,HL                          |*     |*     |?     |V     |1     |*     |ED 62 |      |       |15      |Subtract register pair HL from HL with carry.                |
|SBC HL,SP                          |*     |*     |?     |V     |1     |*     |ED 72 |      |       |15      |Subtract register pair SP from HL with carry.                |
|SBC L                              |*     |*     |?     |V     |1     |*     |9D    |      |       |4       |Subtract register r from accumulator with carry.             |
|SCF                                |      |      |0     |      |0     |1     |37    |      |       |4       |Set carry flag (C=1).                                        |
|SET 0,(HL)                         |      |      |      |      |      |      |CB C6 |      |       |15      |Set bit b of location (HL).                                  |
|SET 0,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |C6     |23      |Set bit b of location (IX+N).                                |
|SET 0,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |C6     |23      |Set bit b of location (IY+N).                                |
|SET 0,A                            |      |      |      |      |      |      |CB C7 |      |       |8       |Set bit b of register r.                                     |
|SET 0,B                            |      |      |      |      |      |      |CB C0 |      |       |8       |Set bit b of register r.                                     |
|SET 0,C                            |      |      |      |      |      |      |CB C1 |      |       |8       |Set bit b of register r.                                     |
|SET 0,D                            |      |      |      |      |      |      |CB C2 |      |       |8       |Set bit b of register r.                                     |
|SET 0,E                            |      |      |      |      |      |      |CB C3 |      |       |8       |Set bit b of register r.                                     |
|SET 0,H                            |      |      |      |      |      |      |CB C4 |      |       |8       |Set bit b of register r.                                     |
|SET 0,L                            |      |      |      |      |      |      |CB C5 |      |       |8       |Set bit b of register r.                                     |
|SET 1,(HL)                         |      |      |      |      |      |      |CB CE |      |       |15      |Set bit b of location (HL).                                  |
|SET 1,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |CE     |23      |Set bit b of location (IX+N).                                |
|SET 1,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |CE     |23      |Set bit b of location (IY+N).                                |
|SET 1,A                            |      |      |      |      |      |      |CB CF |      |       |8       |Set bit b of register r.                                     |
|SET 1,B                            |      |      |      |      |      |      |CB C8 |      |       |8       |Set bit b of register r.                                     |
|SET 1,C                            |      |      |      |      |      |      |CB C9 |      |       |8       |Set bit b of register r.                                     |
|SET 1,D                            |      |      |      |      |      |      |CB CA |      |       |8       |Set bit b of register r.                                     |
|SET 1,E                            |      |      |      |      |      |      |CB CB |      |       |8       |Set bit b of register r.                                     |
|SET 1,H                            |      |      |      |      |      |      |CB CC |      |       |8       |Set bit b of register r.                                     |
|SET 1,L                            |      |      |      |      |      |      |CB CD |      |       |8       |Set bit b of register r.                                     |
|SET 2,(HL)                         |      |      |      |      |      |      |CB D6 |      |       |15      |Set bit b of location (HL).                                  |
|SET 2,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |D6     |23      |Set bit b of location (IX+N).                                |
|SET 2,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |D6     |23      |Set bit b of location (IY+N).                                |
|SET 2,A                            |      |      |      |      |      |      |CB D7 |      |       |8       |Set bit b of register r.                                     |
|SET 2,B                            |      |      |      |      |      |      |CB D0 |      |       |8       |Set bit b of register r.                                     |
|SET 2,C                            |      |      |      |      |      |      |CB D1 |      |       |8       |Set bit b of register r.                                     |
|SET 2,D                            |      |      |      |      |      |      |CB D2 |      |       |8       |Set bit b of register r.                                     |
|SET 2,E                            |      |      |      |      |      |      |CB D3 |      |       |8       |Set bit b of register r.                                     |
|SET 2,H                            |      |      |      |      |      |      |CB D4 |      |       |8       |Set bit b of register r.                                     |
|SET 2,L                            |      |      |      |      |      |      |CB D5 |      |       |8       |Set bit b of register r.                                     |
|SET 3,(HL)                         |      |      |      |      |      |      |CB DE |      |       |15      |Set bit b of location (HL).                                  |
|SET 3,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |DE     |23      |Set bit b of location (IX+N).                                |
|SET 3,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |DE     |23      |Set bit b of location (IY+N).                                |
|SET 3,A                            |      |      |      |      |      |      |CB DF |      |       |8       |Set bit b of register r.                                     |
|SET 3,B                            |      |      |      |      |      |      |CB D8 |      |       |8       |Set bit b of register r.                                     |
|SET 3,C                            |      |      |      |      |      |      |CB D9 |      |       |8       |Set bit b of register r.                                     |
|SET 3,D                            |      |      |      |      |      |      |CB DA |      |       |8       |Set bit b of register r.                                     |
|SET 3,E                            |      |      |      |      |      |      |CB DB |      |       |8       |Set bit b of register r.                                     |
|SET 3,H                            |      |      |      |      |      |      |CB DC |      |       |8       |Set bit b of register r.                                     |
|SET 3,L                            |      |      |      |      |      |      |CB DD |      |       |8       |Set bit b of register r.                                     |
|SET 4,(HL)                         |      |      |      |      |      |      |CB E6 |      |       |15      |Set bit b of location (HL).                                  |
|SET 4,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |E6     |23      |Set bit b of location (IX+N).                                |
|SET 4,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |E6     |23      |Set bit b of location (IY+N).                                |
|SET 4,A                            |      |      |      |      |      |      |CB E7 |      |       |8       |Set bit b of register r.                                     |
|SET 4,B                            |      |      |      |      |      |      |CB E0 |      |       |8       |Set bit b of register r.                                     |
|SET 4,C                            |      |      |      |      |      |      |CB E1 |      |       |8       |Set bit b of register r.                                     |
|SET 4,D                            |      |      |      |      |      |      |CB E2 |      |       |8       |Set bit b of register r.                                     |
|SET 4,E                            |      |      |      |      |      |      |CB E3 |      |       |8       |Set bit b of register r.                                     |
|SET 4,H                            |      |      |      |      |      |      |CB E4 |      |       |8       |Set bit b of register r.                                     |
|SET 4,L                            |      |      |      |      |      |      |CB E5 |      |       |8       |Set bit b of register r.                                     |
|SET 5,(HL)                         |      |      |      |      |      |      |CB EE |      |       |15      |Set bit b of location (HL).                                  |
|SET 5,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |EE     |23      |Set bit b of location (IX+N).                                |
|SET 5,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |EE     |23      |Set bit b of location (IY+N).                                |
|SET 5,A                            |      |      |      |      |      |      |CB EF |      |       |8       |Set bit b of register r.                                     |
|SET 5,B                            |      |      |      |      |      |      |CB E8 |      |       |8       |Set bit b of register r.                                     |
|SET 5,C                            |      |      |      |      |      |      |CB E9 |      |       |8       |Set bit b of register r.                                     |
|SET 5,D                            |      |      |      |      |      |      |CB EA |      |       |8       |Set bit b of register r.                                     |
|SET 5,E                            |      |      |      |      |      |      |CB EB |      |       |8       |Set bit b of register r.                                     |
|SET 5,H                            |      |      |      |      |      |      |CB EC |      |       |8       |Set bit b of register r.                                     |
|SET 5,L                            |      |      |      |      |      |      |CB ED |      |       |8       |Set bit b of register r.                                     |
|SET 6,(HL)                         |      |      |      |      |      |      |CB F6 |      |       |15      |Set bit b of location (HL).                                  |
|SET 6,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |F6     |23      |Set bit b of location (IX+N).                                |
|SET 6,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |F6     |23      |Set bit b of location (IY+N).                                |
|SET 6,A                            |      |      |      |      |      |      |CB F7 |      |       |8       |Set bit b of register r.                                     |
|SET 6,B                            |      |      |      |      |      |      |CB F0 |      |       |8       |Set bit b of register r.                                     |
|SET 6,C                            |      |      |      |      |      |      |CB F1 |      |       |8       |Set bit b of register r.                                     |
|SET 6,D                            |      |      |      |      |      |      |CB F2 |      |       |8       |Set bit b of register r.                                     |
|SET 6,E                            |      |      |      |      |      |      |CB F3 |      |       |8       |Set bit b of register r.                                     |
|SET 6,H                            |      |      |      |      |      |      |CB F4 |      |       |8       |Set bit b of register r.                                     |
|SET 6,L                            |      |      |      |      |      |      |CB F5 |      |       |8       |Set bit b of register r.                                     |
|SET 7,(HL)                         |      |      |      |      |      |      |CB FE |      |       |15      |Set bit b of location (HL).                                  |
|SET 7,(IX+n)                       |      |      |      |      |      |      |DD CB |XX    |FE     |23      |Set bit b of location (IX+N).                                |
|SET 7,(IY+n)                       |      |      |      |      |      |      |FD CB |XX    |FE     |23      |Set bit b of location (IY+N).                                |
|SET 7,A                            |      |      |      |      |      |      |CB FF |      |       |8       |Set bit b of register r.                                     |
|SET 7,B                            |      |      |      |      |      |      |CB F8 |      |       |8       |Set bit b of register r.                                     |
|SET 7,C                            |      |      |      |      |      |      |CB F9 |      |       |8       |Set bit b of register r.                                     |
|SET 7,D                            |      |      |      |      |      |      |CB FA |      |       |8       |Set bit b of register r.                                     |
|SET 7,E                            |      |      |      |      |      |      |CB FB |      |       |8       |Set bit b of register r.                                     |
|SET 7,H                            |      |      |      |      |      |      |CB FC |      |       |8       |Set bit b of register r.                                     |
|SET 7,L                            |      |      |      |      |      |      |CB FD |      |       |8       |Set bit b of register r.                                     |
|SLA (HL)                           |*     |*     |0     |P     |0     |*     |CB 26 |      |       |15      |Shift value at location (HL) left arithmetic.                |
|SLA (IX+n)                         |*     |*     |0     |P     |0     |*     |DD CB |XX    |26     |23      |Shift value at location (IX+N) left arithmetic.              |
|SLA (IY+n)                         |*     |*     |0     |P     |0     |*     |FD CB |XX    |26     |23      |Shift value at location (IY+N) left arithmetic.              |
|SLA A                              |*     |*     |0     |P     |0     |*     |CB 27 |      |       |8       |Shift register r left arithmetic.                            |
|SLA B                              |*     |*     |0     |P     |0     |*     |CB 20 |      |       |8       |Shift register r left arithmetic.                            |
|SLA C                              |*     |*     |0     |P     |0     |*     |CB 21 |      |       |8       |Shift register r left arithmetic.                            |
|SLA D                              |*     |*     |0     |P     |0     |*     |CB 22 |      |       |8       |Shift register r left arithmetic.                            |
|SLA E                              |*     |*     |0     |P     |0     |*     |CB 23 |      |       |8       |Shift register r left arithmetic.                            |
|SLA H                              |*     |*     |0     |P     |0     |*     |CB 24 |      |       |8       |Shift register r left arithmetic.                            |
|SLA L                              |*     |*     |0     |P     |0     |*     |CB 25 |      |       |8       |Shift register r left arithmetic.                            |
|SRA (HL)                           |*     |*     |0     |P     |0     |*     |CB 2E |      |       |15      |Shift value at location (HL) right arithmetic.               |
|SRA (IX+n)                         |*     |*     |0     |P     |0     |*     |DD CB |XX    |2E     |23      |Shift value at location (IX+N) right arithmetic.             |
|SRA (IY+n)                         |*     |*     |0     |P     |0     |*     |FD CB |XX    |2E     |23      |Shift value at location (IY+N) right arithmetic.             |
|SRA A                              |*     |*     |0     |P     |0     |*     |CB 2F |      |       |8       |Shift register r right arithmetic.                           |
|SRA B                              |*     |*     |0     |P     |0     |*     |CB 28 |      |       |8       |Shift register r right arithmetic.                           |
|SRA C                              |*     |*     |0     |P     |0     |*     |CB 29 |      |       |8       |Shift register r right arithmetic.                           |
|SRA D                              |*     |*     |0     |P     |0     |*     |CB 2A |      |       |8       |Shift register r right arithmetic.                           |
|SRA E                              |*     |*     |0     |P     |0     |*     |CB 2B |      |       |8       |Shift register r right arithmetic.                           |
|SRA H                              |*     |*     |0     |P     |0     |*     |CB 2C |      |       |8       |Shift register r right arithmetic.                           |
|SRA L                              |*     |*     |0     |P     |0     |*     |CB 2D |      |       |8       |Shift register r right arithmetic.                           |
|SRL (HL)                           |*     |*     |0     |P     |0     |*     |CB 3E |      |       |15      |Shift value at location (HL) right logical.                  |
|SRL A                              |*     |*     |0     |P     |0     |*     |CB 3F |      |       |8       |Shift register r right logical.                              |
|SRL B                              |*     |*     |0     |P     |0     |*     |CB 38 |      |       |8       |Shift register r right logical.                              |
|SRL C                              |*     |*     |0     |P     |0     |*     |CB 39 |      |       |8       |Shift register r right logical.                              |
|SRL D                              |*     |*     |0     |P     |0     |*     |CB 3A |      |       |8       |Shift register r right logical.                              |
|SRL E                              |*     |*     |0     |P     |0     |*     |CB 3B |      |       |8       |Shift register r right logical.                              |
|SRL H                              |*     |*     |0     |P     |0     |*     |CB 3C |      |       |8       |Shift register r right logical.                              |
|SRL L                              |*     |*     |0     |P     |0     |*     |CB 3D |      |       |8       |Shift register r right logical.                              |
|SUB (HL)                           |*     |*     |*     |V     |1     |*     |96    |      |       |7       |Subtract location (HL) from accumulator.                     |
|SUB (IX+n)                         |*     |*     |*     |V     |1     |*     |DD 96 |XX    |       |19      |Subtract location (IX+N) from accumulator.                   |
|SUB (IY+n)                         |*     |*     |*     |V     |1     |*     |FD 96 |XX    |       |19      |Subtract location (IY+N) from accumulator.                   |
|SUB A                              |*     |*     |*     |V     |1     |*     |97    |      |       |4       |Subtract register r from accumulator.                        |
|SUB B                              |*     |*     |*     |V     |1     |*     |90    |      |       |4       |Subtract register r from accumulator.                        |
|SUB C                              |*     |*     |*     |V     |1     |*     |91    |      |       |4       |Subtract register r from accumulator.                        |
|SUB D                              |*     |*     |*     |V     |1     |*     |92    |      |       |4       |Subtract register r from accumulator.                        |
|SUB E                              |*     |*     |*     |V     |1     |*     |93    |      |       |4       |Subtract register r from accumulator.                        |
|SUB H                              |*     |*     |*     |V     |1     |*     |94    |      |       |4       |Subtract register r from accumulator.                        |
|SUB L                              |*     |*     |*     |V     |1     |*     |95    |      |       |4       |Subtract register r from accumulator.                        |
|SUB n                              |*     |*     |*     |V     |1     |*     |D6    |XX    |       |7       |Subtract value n from accumulator.                           |
|XOR (HL)                           |*     |*     |*     |P     |0     |0     |AE    |      |       |7       |Exclusive OR value at location (HL) and accumulator.         |
|XOR (IX+n)                         |*     |*     |*     |P     |0     |0     |DD AE |XX    |       |19      |Exclusive OR value at location (IX+N) and accumulator.       |
|XOR (IY+n)                         |*     |*     |*     |P     |0     |0     |FD AE |XX    |       |19      |Exclusive OR value at location (IY+N) and accumulator.       |
|XOR A                              |*     |*     |*     |P     |0     |0     |AF    |      |       |4       |Exclusive OR register r and accumulator.                     |
|XOR B                              |*     |*     |*     |P     |0     |0     |A8    |      |       |4       |Exclusive OR register r and accumulator.                     |
|XOR C                              |*     |*     |*     |P     |0     |0     |A9    |      |       |4       |Exclusive OR register r and accumulator.                     |
|XOR D                              |*     |*     |*     |P     |0     |0     |AA    |      |       |4       |Exclusive OR register r and accumulator.                     |
|XOR E                              |*     |*     |*     |P     |0     |0     |AB    |      |       |4       |Exclusive OR register r and accumulator.                     |
|XOR H                              |*     |*     |*     |P     |0     |0     |AC    |      |       |4       |Exclusive OR register r and accumulator.                     |
|XOR L                              |*     |*     |*     |P     |0     |0     |AD    |      |       |4       |Exclusive OR register r and accumulator.                     |
|XOR n                              |*     |*     |*     |P     |0     |0     |EE    |XX    |       |7       |Exclusive OR value n and accumulator.                        |
