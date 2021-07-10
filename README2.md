# Transactions

1. The Structure of a Transaction
2. The Transaction Nonce
  2.1. Keeping Track of Nonces
3. Transaction Gas
4. Transaction Recipient
5. Transaction Value and Data
6. Special Transaction: Contract Creation
7. Digital Signatures
8. The Signature Prefix Value (v) and Public Key Recovery
9. Separating Signing and Transmission (Offline Signing)
10. Transaction Propagation
11. Recording on the Blockchain
12. Multiple-Signature (Multisig) Transactions
13. Conclusions



서문: ' 서문 '  
1장: ' 이더리움이란 무엇인가 '  
  ->  **분산 시스템**으로 작동 (  스마트 계약에 대한 액세스를 제어하는 ​​개인 키를 제어할 수 있고 제어 )  
  ->  **탈중앙화**된 세계 컴퓨터로서의 이더리움의 기능에 종속 ( 이더리움 블록체인 )  
  ->   
  ** 1장 용어 **  
  -> 자금에 대한 접근과 스마트 계약의 조합을 "계정" 또는 "지갑"  
  -> 그러나 기본 원칙으로서 하나의 개인 키가 하나의 "계정"과 동일
2장: ' 이더리움 기초 '  
  -> 지갑을 사용하는 방법, 트랜잭션을 생성하는 방법 및 기본 스마트 계약을 실행하는 방법  
  -> 1, 이더리움 블록체인는 월드 컴퓨터에서 작동.  
  -> 2. 외부 소유 계정(EOA) 및 계약  
      - MetaMask 지갑에서 생성한 계정 유형을 **외부 소유 계정 (EOA)** ( 외부 소유 계정은 **개인 키**가 있는 계정. 즉, 인 키가 있다는 것은 자금 또는 계약에 대한 **액세스를 제어한다**  
         는 의미 )  
      - **계약 계정** ( 계약 계정에는 간단한 EOA가 가질 수 없는 스마트 계약 코드가 있습니다. 계약 계정에는 개인 키가 없습니다. 대신 스마트 계약 코드의 논리에 의해 소유(및 제어)됩니다. 계약         계정생성 시 **이더리움 블록체인에 기록되고 EVM에 의해 실행되는 소프트웨어 프로그램** )  
      - MetaMask vs 계약 계정 ( 계약에는 EOA와 마찬가지로 주소가 있습니다. 계약은 EOA와 마찬가지로 **이더를 보내고 받을 수도 있습니다.**  
        그러나 트랜잭션 대상이 **계약 주소인 경우** 트랜잭션과 트랜잭션 데이터를 입력으로 사용하여 해당 계약 이 EVM에서 실행 됩니다  
        계약 계정에는 개인 키가 없기 때문에 트랜잭션을 시작할 수 없습니다  
        **EOA만 트랜잭션을 시작할 수 있지만** **계약은 다른 계약을 호출하고 복잡한 실행 경로를 구축하여 트랜잭션에 반응 할 수 있습니다**  
        **일반적인 DApp 프로그래밍 패턴은 계약 A의 사용자 간에 공유 상태를 유지하기 위해 계약 A가 계약 B를 호출하도록 하는 것입니다.**  
        )   
          
  -> 3. 계약 컴파일 ( 컴파일러를 사용하여 Solidity 코드를 블록체인 자체의 **EVM에서 실행할 수 있도록 EVM 바이트 코드로 변환** )  
  -> 5. 블록체인에서 계약 생성  
      - 이제 **이더리움 블록체인에** **계약을 "등록"**  
      - **블록체인에 계약을 등록하려면 대상이 주소 0x00000000000000000000000000000000000000( 영 주소 라고도 함)인 특수 트랜잭션을 생성**  
      ( 이더리움 블록체인에 계약을 등록하고 싶다는 것을 알려주는 특별한 주소 )  
    
3장: ' 이더리움 클라이언트 '  
4장: ' 암호화 '  
5장: ' 지갑 '  
6장: ' 거래 '
7장: ' 스마트 계약과 견고성 '  
8장: ' 스마트 계약과 바이퍼 '  
9장: ' 스마트 계약 보안 '  
10장: ' 토큰 '  
11장: ' 오라클 '  
12장: ' 분산 애플리케이션(DApps) '  
13장: ' 이더리움 가상 머신 '  
14장: ' 합의 '  
  
트렌젝션
- 블록체인
- 거래
- 
- 거래는 외부 소유 계정 (EOA)에서 생성되고 이더 리움 네트워크에 의해 전송되고 이더 리움 블록 체인에 기록 된 서명 된 메시지입니다.
-  트랜잭션을 보는 또 다른 방법은 트랜잭션이 상태 변경을 트리거하거나 계약이 EVM에서 실행되도록 할 수있는 유일한 것입니다.
-  이더 리움은 글로벌 싱글 톤 상태 머신이며 

## 1.The Structure of a Transaction

## 2.The Transaction Nonce

### 2.1. Keeping Track of Nonces

## 3. Transaction Gas

## 4. Transaction Recipient

## 5. Transaction Value and Data

## 6. Special Transaction: Contract Creation

## 7. Digital Signatures

## 8. The Signature Prefix Value (v) and Public Key Recovery

## 9. Separating Signing and Transmission (Offline Signing)

## 10. Transaction Propagation

## 11. Recording on the Blockchain

## 12. Multiple-Signature (Multisig) Transactions

## 13. Conclusions
