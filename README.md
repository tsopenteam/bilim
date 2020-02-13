# bilim - Teknoseyir Teknoloji ve Bilim Notları

### Teknoloji ve Bilim Notları Nedir ?

> teknoseyir.com tarafından yapılan, teknoloji ve bilim ile ilgili konuların konuşulduğu bir programdır.
> Olabildiğince her hafta yayınlanır.

### bilim.json Nedir ?

> Yayınlanan tüm bilim bilgilerinin kayıt altına alındığı proje.

### Kullanım

> bilim.json dosyasında tüm bilim notlarını bulabilirsiniz.
> İstediğiniz yerde, istediğiniz şekilde kullanabilirsiniz.
> Yeni yayınlanan bilim notları json dosyasına eklenmektedir.

### Json Veri Yapısı

```typescript
declare module namespace {

    export interface Content {
        contentText: string;
        contentLink: string[];
    }

    export interface List {
        year: string;
        count: number;
        totalCount: number;
        uploadDate: string;
        podcastLink: string;
        videoLink: string;
        siteLink: string;
        titlePodcast: string;
        explanationPodcast: string;
        content: Content[];
    }

    export interface RootObject {
        list: List[];
    }

}
```