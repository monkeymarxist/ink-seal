INK & SEAL
by Monkey Marxist

A static, browser-only PDF signature and stamp editor.

Ink-and-Seal.html is a self-contained edition with every library, font, and
character map embedded. Save it to your computer and open it in a current
browser. The app requires no internet connection for processing. Browser
storage support for local files varies; the app reports any storage failure.

The standalone edition has been functionally checked through a local HTTP
preview. Direct file opening could not be browser-tested in this environment.

Ink-and-Seal.zip contains the separate editable HTML, CSS, JavaScript, and
vendor files for static hosting.

1. Open the app. Choose Add signature or Add stamp.
2. Upload a JPG/PNG photograph, or use Take a photo on a phone.
3. Drag over the original photo to crop to the required signature or stamp.
4. Adjust Paper cleanup until the checkerboard shows through the empty paper.
   Keep Ink strength at 100% to preserve natural ink density. Brightness,
   contrast, saturation, and sharpness update the transparent preview live.
   Reset adjustments returns those four settings to their defaults.
5. Turn on Pixel eraser and brush over stray marks in the transparent preview.
   Brush size is measured in image pixels, from 1 to 80. Zoom to 100%, 200%,
   or 400% for precise cleanup; scroll inside the preview to reach more ink.
   Turn the eraser off to pan a zoomed preview with one finger.
   Undo restores the last stroke (up to 25 strokes), and Restore erased ink
   restores all erased pixels in the current editing session. Erasures stay
   aligned when you change the crop, cleanup, or image adjustments.
6. Save the ink, open a PDF, and click your saved ink to place it.
7. Drag to move. Use the lower-right corner to resize. Drag the round handle
   above a selected image to rotate with a mouse or one finger. Hold Shift
   while dragging for 15-degree snapping. For precise rotation, focus the
   round handle and use arrow keys for 0.1-degree steps, Shift + arrow for
   1-degree steps, and Home to reset. Rotation is kept in the exported PDF.
   Use the small buttons beside a selected image to duplicate or remove it.
8. Switch pages and add further copies as needed, then Download PDF.
9. To clean ink already saved in the library, use its pencil button. Save
   changes updates that library item. Place it again to use the new version;
   copies already on a PDF keep the image they had when placed.

All document and image processing happens locally in the browser. Signatures
and stamps are stored as transparent PNG data in IndexedDB, tied to this site
and browser profile. Clearing browser data clears the library. Download a PNG
backup using the download button below a saved item.

PDF placements exist during the editing session. Download your PDF before
closing or replacing it. The original PDF is preserved in memory and ink is
embedded into a new PDF on export. These are visual ink images.

For best results, use a close-up photograph on smooth white paper in even
lighting. The adjustable cleanup removes paper colour and shadows while
preserving soft ink edges. Erasing clears pixels to full transparency.
Deep wrinkles, harsh shadows, or blur may require
a clearer photograph or tighter crop. JPG, PNG, WEBP, and browser-supported
camera image formats are accepted. PDFs must be unlocked and under 50 MB.

HOSTING THE INCLUDED FILES

Extract Ink-and-Seal.zip and place the contents on any static HTTPS web host.
index.html is the entry point. Keep the vendor folder beside it. There is no
backend, server-side scripting, npm installation, or build step. All PDF
libraries, character maps, and fonts are included locally.

Use an HTTP/HTTPS URL. Browsers restrict JavaScript modules opened through a
file:// URL, so double-clicking index.html is not a supported launch method.
For a local preview, serve the folder with any ordinary static file server.

The included libraries are PDF.js 4.10.38 (Apache 2.0) and pdf-lib 1.17.1 (MIT).
Their license files are in vendor/.
