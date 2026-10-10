# 🎙️ Textify

> An integrated accessibility-focused application for converting between speech, text, images, and video content.

Textify is a cross-platform application that brings multiple media-processing features together in a single interface. It supports **Speech-to-Text, Text-to-Speech, OCR, and YouTube caption generation**, making text and audio content easier to access and manage.

## ✨ Features

- 🎤 **Speech-to-Text** — Convert spoken audio into text using Google Speech-to-Text.
- 🔊 **Text-to-Speech** — Convert written text into speech using Google Text-to-Speech.
- 📷 **OCR** — Extract editable text from images using Google ML Kit.
- ▶️ **YouTube Captions** — Extract and generate text from YouTube videos using their URLs.
- 📱 **Cross-Platform** — Built with Flutter for multi-platform support.
- ⚡ **Backend Processing** — Python and FastAPI backend for media-processing tasks.

## 🏗️ Architecture

```text
                    ┌─────────────────────┐
                    │    Flutter App      │
                    │   Cross-Platform    │
                    └──────────┬──────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
              ▼                ▼                ▼
        Speech-to-Text    Text-to-Speech       OCR
              │                │                │
              └────────────────┼────────────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    FastAPI Backend  │
                    │  Python Processing  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ YouTube Captions    │
                    └─────────────────────┘