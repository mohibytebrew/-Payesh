FROM node:18-bullseye

RUN apt-get update && apt-get install -y \
    build-essential \
    libcairo2-dev \
    libpango1.0-dev \
    libjpeg-dev \
    libgif-dev \
    librsvg2-dev \
    python3 \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /app

COPY src/package.json src/package-lock.json* ./
RUN npm install

COPY src/ .

EXPOSE 9990 10000

CMD ["npm", "start"]

