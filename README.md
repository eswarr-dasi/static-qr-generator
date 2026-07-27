# Static QR Code Generator

A free, single-page QR code generator that runs entirely in your browser. No signup, no account, no server, no tracking, and no expiration.

Live site: https://eswarr-dasi.github.io/static-qr-generator/

## What it does

Generates QR codes for a website URL, plain text, an email address, a phone number, or a Wi-Fi network. You can pick the output size, error correction level, and QR/background colors, then download the result as a PNG. Everything happens client-side using the QRCode.js library loaded from a CDN; the data you type never leaves your browser or touches a server.

## Why this exists

Most QR generators fall into two camps: paid tools gated behind signup, or free "dynamic QR" services that route the code through their own redirect server. That second category has a real downside people complain about online: the underlying short link can expire, get paywalled later, or quietly track every scan, which breaks the QR code even though the printed image never changes. This tool takes the opposite approach. It encodes your content directly into the QR code itself, so once it is generated it works forever, with no dependency on this site or any other server staying online.

## Status

Freshly built and live. Core flows have been tested by generating a QR code and decoding it back to verify the encoded data is exactly correct for URL, Wi-Fi (including special characters in the password), and phone number types. This is a brand new site with no search ranking yet, so traffic will take time to build the same way it does for any new page on the web.

## Ideas for later

Possible additions include a vCard/contact-card QR type, an SVG download option alongside PNG, and a batch mode for generating several QR codes at once.
