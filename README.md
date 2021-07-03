# NOT For Review Just keeping my useful thing.. :)

# Angular
<a href="https://stackblitz.com/edit/angular-ngx-leaflet-tests-3p74ln?file=dialog/example-dialog.component.ts">Angular View understanding</a>


# Node.js
<a href="https://stackoverflow.com/questions/50371593/angular-6-uncaught-referenceerror-buffer-is-not-defined">Convert into Blob</a>
------Choose Image from google drive.
service.ts
async downloadFile(fileId: string, mimeType: string) {
    const res = await gapi.client.drive.files.get({
      fileId,
      alt: 'media'
    });
    const base64 = 'data:' + mimeType + ';base64,' + Buffer.from(res.body, 'binary').toString('base64');
    return base64;
  }
component.ts
downloadFile(id: any, mimeType: any) {
    this.driveService.downloadFile(id, mimeType)
      .then(val => {
        console.log(val);
      });
  }
  ------convert into base64.
  
  # React 
  <ul>
  <a href="https://codesandbox.io/s/es6-spread-operator-practice-forked-4m276">Rendering list of notes *.*</a>
  <a href="https://rd7gy.csb.app/">How can we delete the exsisting list items.*.*</a>
</ul>
