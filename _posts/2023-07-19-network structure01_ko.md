---
layout: post
title: 네트워크 구조에 대하여
subtitle: VM네트워크 설정을 하기전, bridged, Host-only 그리고 NAT에 대하여 알아봅시다.
author: SH-Kwon
categories: Network
banner:
  loop: true
  volume: 0.8
  start_at: 8.5
  opacity: 0.618
  background: "#000"
  height: "100vh"
  min_height: "38vh"
  heading_style: "font-size: 4.25em; font-weight: bold; text-decoration: underline"
  subheading_style: "color: MediumAquamarine"
tags: network
sidebar: []
---

VM(Virtual Machine)을 구성하기 이전에, 각 VM이 사용할 네트워크 어댑터의 구성방식에 대해 알아볼 필요가 있다.
네트워크의 구성방식은 bridged, Host-only, NAT로 나뉜다.

1. Bridged
브릿지 네트워크는 실제 물리적으로 존재하는 호스트 머신의 네트워크 어댑터와 VM의 네트워크 어댑터가 직접적으로 연결되는 네트워크 구성방식이다.

default 값으로 vmnet0은 자동 bridged모드를 사용하게 설정되어 있으며, 호스트 시스템상에 액티브 상태인 모든 네트워크 어댑터에 브릿지로 접속된다.
물론 VMNet editor를 이용해 vmnet0을 bridged에서 다른 네트워크로 변경하는 것도 가능하나 이런 설정 변경은 호스트 시스템에서 bridged 네트워크를 사용하는 모든 가상머신에 영향을 미친다.


2. Host-only
외부와 격리된 가상 네트워크를 구축할 때 사용한다. 즉, 외부의 인터넷 연결이 필요가 없을 때 사용한다.
Host-only에서는 
기본적인 구성으로는 host-only 네트워크의 가상머신은 외부 인터넷 접속이 불가능하다.

3. NAT
NAT에서는 가상 머신들이 공인아이피를 가지지 않는 대신, 호스트 시스템 내부에 구축된 별도의 사설 네트워크의 아이피를 가진다.
**oracle VM virtualBox에서는 NAT가 default networking mode이다.