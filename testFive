// SPDX-License-Identifier: MIT
pragma solidity 0.8.13;


contract A {

// Using other contracts



    string private start = "one";


    function getValue() public view returns(string memory){
        return start;
    }


    function changeValue(string calldata change) public{
        start = change;
    }


}
// SPDX-License-Identifier: MIT
pragma solidity 0.8.13;


interface IA{
    function getValue() external view returns(string memory);
    function changeValue(string memory) external;


}


contract B{








    function getValue() public view returns(string memory){
        IA contractA = IA(0x0000000000000000000000000000000000000000);


        return contractA.getValue();


    }


    function changeValue(string memory changeStart) public{
        IA contractA = IA(0x0000000000000000000000000000000000000000);


        contractA.changeValue(changeStart);


    }
}
