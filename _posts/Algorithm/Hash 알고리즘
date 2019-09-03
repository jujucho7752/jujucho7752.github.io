---
layout: post
title: Hash 알고리즘 _ 완주하지 못한 선수의 이름
description: ""
modified: 2016-06-01T15:27:45-04:00
tags: [programmers,code, java, hash , javascript]
image:
  path: /images/abstract-10.jpg
  feature: abstract-10.jpg
---

[programmers][Java]
## Hash 알고리즘
완주하지 못한 선수의 이름

### 내 코드

import java.util.HashMap;
import java.util.Map;

class Solution {
	public String solution(String[] participant, String[] completion) {
		String answer = "";
		Map<String, Integer> passName = new HashMap<>();
		for (String name : completion) {
			if (passName.containsKey(name))
				passName.put(name, passName.get(name) + 1);
			else
				passName.put(name, 1);
		}
		for (String participantName : participant) {
			if (passName.containsKey(participantName) && passName.get(participantName) > 0) {
				passName.put(participantName, passName.get(participantName) - 1);
			} else {
				answer = participantName;
				break;
			}
		}
		return answer;
	}
}


