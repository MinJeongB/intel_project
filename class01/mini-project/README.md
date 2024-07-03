## Member

* 김민정 B
* 유광균

</br>

## 프로젝트 개요

**외식 물가 상승에 따라 집 밥 수요가 증가  ->  요리에 도움을 줄 수 있는 시스템 고안**

외식 물가가 고공행진하면서 밀폐용기가 불티나게 팔리고 있는 것으로 나타났다.</br>
집에서 끼니를 해결하려는 수요가 폭발적으로 늘어난 데 따른 것이다.</br> https://www.asiae.co.kr/article/2024021321252712891

</br>

## 프로젝트 소개

**" 재료 준비 도우미 "</br>
: 요리를 하기에 앞서, 준비된 재료가 올바른지 확인하기 위해 음식 재료를 확인해주는 시스템**

* 사용 모델</br>
openvino eng OCR : 설탕, 소금, 밀가루, 부침가루 등과 같이 외관으로 구별 불가능한 제품을 text 로 확인</br>
Object Detetion : 외관으로 구별 가능한 제품은 Detetion 으로 확인

</br>

## 프로젝트 목표

* 프로젝트 목표
 현재 준비된 음식 재료가 무엇인지 확인
 최종 프로젝트 기술 선별 학습
 
* 기술적 부분
 ocr 개념 정리
 한국어 ocr 모델 구현 선행 학습
 OCR & Object Detection 두 가지 모델 병합

</br>

## 시스템 구성도

![구성도](https://cdn.discordapp.com/attachments/1247775254416326708/1250358636354605137/e077158d41eb8280.png?ex=6685ad79&is=66845bf9&hm=cef64a29bccec0bd878534d339d63f2361454416e83e7f82908ab06f872228e5&)

</br>

## 시연 및 결과

![캡처 이미지1](https://cdn.discordapp.com/attachments/1249972873104199710/1250306765736644690/Screenshot_from_2024-06-12_13-32-35.png?ex=66857d2a&is=66842baa&hm=62ff54bb5129d9743de5b4442adeb4c327c1619128eff28a720995c8553b4dc5&)
![캡처 이미지2](https://cdn.discordapp.com/attachments/1249972873104199710/1250307270940819529/Screenshot_from_2024-06-12_13-34-35.png?ex=66857da2&is=66842c22&hm=b900f5deed6959bbc7ca5ea41710d62610b012893579d7eda101a4fa10c254bc&)

</br>

## 고찰 및 보완점

**1. 한국어 ocr 구현**
- 데이터 전처리 수행 후 직접 ocr 모델 구현
- 구현 실패 시, </br>방법 1 : 한글 detection 후 pytesseract 라이브러리 활용</br>
 방법 2 : EasyOCR 라이브러리 활용
</br>
**2. 웝캠 실시간 detection & ocr 구현** 
</br>
