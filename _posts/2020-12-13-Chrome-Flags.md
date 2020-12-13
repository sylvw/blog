---
layout: post
title: Today I learned - --disable-dev-shm-usage chrome flag
---
Background: Tests written with webdriverio started to fail in CI
(This is WIP description.)
Issue: 
returned by webdriverio: "invalid session id"
after debugging: "WARN webdriver: Request failed with status 500 due to unknown error: session deleted because of page crash
from tab crashed" 

Solution: --disable-dev-shm-usage flag added to chromeOptions can fix a problem 

#webdriverio #docker #centos #chrome