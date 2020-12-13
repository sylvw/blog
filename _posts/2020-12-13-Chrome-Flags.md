---
layout: post
title: --disable-dev-shm-usage chrome flag
---
(This is WIP description.)

Background: Tests written with webdriverio started to fail in CI

Issue: 
returned by webdriverio: "invalid session id"

after debugging: "WARN webdriver: Request failed with status 500 due to unknown error: session deleted because of page crash
from tab crashed" 

Solution: --disable-dev-shm-usage flag added to chromeOptions can fix a problem 

#webdriverio #docker #centos #chrome