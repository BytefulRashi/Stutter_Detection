# Stutter Detection Application

## Overview
A machine learning-based application that detects and analyzes stuttering patterns in speech by combining audio and textual analysis. The system provides detailed feedback to help individuals track and improve their speech patterns.

## Technical Architecture

### Input Processing
- **Audio Input**: Accepts WAV format audio recordings
- **Dual-Stream Processing**: 
  - Stream 1: Audio-to-text conversion for linguistic analysis
  - Stream 2: Direct audio signal processing for acoustic analysis

### Core Components
1. **Wav2Vec Conversion**
   - Transforms raw audio into matrix representations
   - Processes both transcribed text and direct voice signals

2. **Text Processing**
   - Generates text transcriptions from audio
   - Utilizes Agnostic BERT for contextual embedding
   - Creates vector embeddings for semantic analysis

3. **Vector Integration**
   - Concatenates audio and text embeddings
   - Creates unified feature vectors for classification

4. **Classification System**
   - Employs a binary classifier to identify stuttering patterns
   - Outputs: stutterer/non-stutterer classification

### Features
- Real-time stuttering detection
- Percentage calculation of stuttering instances
- Temporal marking of stuttering events
- Pattern recognition of specific stuttering types
- Detailed analysis report generation

## Applications
- Speech therapy support tool
- Self-paced practice environment
- Progress tracking and monitoring
- Educational resource for speech pathologists

## Technical Requirements
- Compatible with WAV audio format
- Python environment with deep learning capabilities
- Required libraries:
  - Wav2Vec
  - BERT
  - Audio processing libraries

## Goals and Impact
- Provide objective analysis of speech patterns
- Enable data-driven speech improvement
- Support speech therapy professionals
- Enhance communication confidence
- Create accessible tools for speech improvement
