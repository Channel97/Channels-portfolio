# RE:DEFINE Final Portfolio

Docker-ready static portfolio site with glass UI, animated transitions, portfolio filters, video showcase, credentials and drag-and-drop asset folders.

## Run locally

```bash
docker build -t redefine-final .
docker run -d -p 8092:80 --name redefine-final redefine-final
```

Open: http://localhost:8092

## Replace assets

Keep the same filenames for fastest editing:

- assets/hero/slide1.jpg, slide2.jpg, slide3.jpg — 1920x1080
- assets/social/post1.jpg to post6.jpg — 1080x1080
- assets/web/site1.jpg to site3.jpg — 1400x900
- assets/print/print1.jpg and print2.jpg — 1920x1080
- assets/videos/showreel.mp4 — MP4 video
- assets/accreditation/degree.pdf — Degree PDF
- assets/accreditation/portfolio.pdf — Portfolio PDF

## Rebuild after changes

```bash
docker rm -f redefine-final
docker build -t redefine-final .
docker run -d -p 8092:80 --name redefine-final redefine-final
```
