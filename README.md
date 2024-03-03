# one_point_five
## Pull in the latest image from docker. Supports both amd64 and arm64 CPU architectures.
```bash
docker pull mintplexlabs/anythingllm
```
Linux/MacOs(commands)
```bash
export STORAGE_LOCATION=$HOME/anythingllm && \
mkdir -p $STORAGE_LOCATION && \
touch "$STORAGE_LOCATION/.env" && \
docker run -d -p 3001:3001 \
--cap-add SYS_ADMIN \
-v ${STORAGE_LOCATION}:/app/server/storage \
-v ${STORAGE_LOCATION}/.env:/app/server/.env \
-e STORAGE_DIR="/app/server/storage" \
mintplexlabs/anythingllm
```
**your llm is set now**

