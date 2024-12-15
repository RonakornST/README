# cs-dlp Installation and Usage Guide

## Installation


Follow these steps to install `cs-dlp`:

1. Clone the repository:
   ```bash
   git clone https://github.com/raffaem/cs-dlp
   ```

2. Navigate into the repository directory:
   ```bash
   cd cs-dlp
   ```

3. Install the tool using pip:
   ```bash
   pip3 install .
   ```

---

## How to Download a Course

The basic command format is:

```bash
cs-dlp -ca {CAUTH_TOKEN} --format "{FILE_FORMATS}" {YOUR_COURSE_NAME}
```

### Parameters:
- **`{CAUTH_TOKEN}`**: Obtain this from your browser's developer tools (explained below).
- **`{FILE_FORMATS}`**: Specify the types of files you want to download (e.g., `mp4`, `pdf`, `pptx`, etc.).
- **`{YOUR_COURSE_NAME}`**: Extract this from the course URL (explained below).

---

### How to Get Your {CAUTH Token}
1. Open the course website in your browser.
2. Use Developer Tools to copy the `CAUTH` token (refer to this video at 2:22 for guidance: [Video Link](https://www.youtube.com/watch?v=fDCln4C0zbI&t=64s)).

---

### How to Find {YOUR_COURSE_NAME}
1. Look at the course URL. For example:
   ```
   https://www.coursera.org/programs/program-8-wchpm/learn/battery-management-systems?authProvider=chulalongkorn-faculty-of-engineering&specialization=algorithms-for-battery-management-systems
   ```
2. The course name appears after `/learn/` and before the `?`. 
   In this example: `battery-management-systems`.

---

## Example Command

Here’s an example of a complete command to download a course:

```bash
cs-dlp -ca XifMIVia4JPHxAmSk0E9zxh_dkIf9x1i_K7L5tkcjcMUolNTZol3BCEI-BqVmd9l-z3XmfpoevigOlLGDOCIWA.wUqSVp5Vo-NBpsKvgmCT_w.3ckKC-Hn6NyVMorBzM92eRET-_KisFQaLipmjrWI8u4jrXk_OypJTpsuyMvyRLpdlK5xR7faPKi5NadBZEjxsOtKz2DIUVowEKXmTpzV_j0L32ZvhELU0y_UUOikmSbFzOI6iXjQW7EJ3zY-KHvpqsravE0CAzrncf4gCQ4mv3uL12VS0a18k1mPL9kUeGi2eoHl9pjeHaSQZNwzGp0gPVXQDpdXhN-nVghzMpdcYi2iJwY-Cfs1eXrUbg_AmBupqW7ZCN6b7huQ089ldtVVRdi67pRn5t9PyM3kd2mXN7F37_mzlcwovQIY8x4Yqgkq9FWffabgbJV0XmFqmiVorYxobt6DJXM-30e4bgMCUTsN5Ddc3yJ5qAfVgyTBAZ6fBqZbGa4XNUedVdny0dh7gFukrn_1t5k9Rjdbxmv9jy4FeCOpYxox7Q9Xs2ej50GacSfCUViE_prit94NSzMs4w \
  --format "mp4 pdf pptx ppt html" \
  --download-quizzes --download-notebooks \
  --video-resolution 720p \
  battery-management-systems
```
## Command with CAUTH that can use until mid jan 2025
```
cs-dlp -ca tAYDKK9-UhvkbIR0sa__AtvGVCw8Jh08pOHJ8cYaDjvj7v5yRZYJCp2quhPB5CS0eWMoglxoM6j7PuezydXYkA.txLTAM-ARQpEIlLlqLl5gw.L5J1v8GZ77ZkLuBk-kkKNBtFkXyDWVr3DqUEAGiExcUxe3HdbvTORy2GcOM_NIlEme7M9hwAeGorvW4Na9jnMwtJXeVje6kBdWbIcLNZUufQ4CyWIolbhKUqiFxo9qgDz9O09QJ3h0jjN_K4B_bnNgP1Bv0iAi2ETLpVXOhVLXCe4ztLK-GyaLmCH8oc2nYSnG9g7icy03QAT2zqJm0SceAs-UE6et6WpV-EKrEpjztg1mbWrE5vimGUM2Q7lRJiZMZpCBni_zsMnWPnBROql1mTrojogmrBAmVarcu264zB7y9Vr2B-rdi8rVG1a5X9yFmqA27CvLxbpXjb5YmcWagWAzBIr1WiZDc5BD00L8wwULNGxadZcqAT38vdkzrLoGgoPn2lJPoK424prYod7QXinjq8WtdCb7TaIpFvt7OQFV_FfXpG3nbRl5V2hj4mfS5BcN0GNHWmdL3rCXXpxA --format "mp4 pdf pptx ppt html"   --download-quizzes --download-notebooks   --video-resolution 720p YOUR_COURSE_NAME
```
---
