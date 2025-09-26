# Container Registry

## What is Container Registry?

**Online storage space for Docker images**

Container Registry serves as a centralized repository where you can store, manage, and distribute Docker images.

## Google Cloud Container Registry

### Docker Hub inside Google Cloud
- Integrated Docker image storage within the Google Cloud ecosystem
- Seamless integration with other GCP services

### Core Operations
You can perform the following operations with Docker images:
- **Store Docker images** - Upload and save images to the registry
- **Pull images** - Download images from the registry
- **Push images** - Upload new or updated images to the registry
- **Tag images** - Apply version tags and labels for organization

## Google Cloud Artifact Registry

### Next-Level Registry Service
**GCP recently introduced next level registry - Artifact Registry**

### Enhanced Capabilities
- **It can store not just Docker images but many more things like NPM, Maven**
- Supports multiple artifact types beyond container images
- Unified repository for various package formats

## Naming Convention

### Standard Format
```
HostName/ProjectID/ImageName:Tag
```

### Example
```
gcr.io/[ProjectID]/nginx:1.0
```

Where:
- `gcr.io` - Google Container Registry hostname
- `[ProjectID]` - Your GCP project identifier
- `nginx` - Image name
- `1.0` - Version tag

## Security and Authorization

### Binary Authorization
- **Binary authorization can be used to detect vulnerabilities & enforce deployment policies**
- Ensures only trusted and secure images are deployed
- Automated security scanning and policy enforcement

### Access Control
- **No IAM Role defined at granular level** - Limited fine-grained access control
- **No Region specific Repository** - Not tied to specific geographic regions

(These two points have already been improved in the Artifact Registry.)

## Pricing Model

**Pricing - store in GCS (Google Cloud Storage)**
- Storage costs are based on Google Cloud Storage pricing
- Pay for the storage space your images consume
- Additional charges may apply for network egress

## Migration Path

```
Docker Hub → Container Registry → Artifact Registry
    ↓              ↓                    ↓
 Public Hub    GCP Container      Multi-format
               Images Only        Package Support
```

Container Registry provides a secure, scalable, and integrated solution for managing container images in Google Cloud Platform, with Artifact Registry offering enhanced capabilities for modern DevOps workflows.
