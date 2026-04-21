# Findings Report

## Summary

The issue involved incorrect DNS resolution caused by a local system configuration.

## Root Cause

A manual entry in the /etc/hosts file redirected the domain to an incorrect IP address.

## Impact

Users were unable to reach the intended destination due to incorrect routing.

## Resolution

The malicious entry was removed from the hosts file, restoring proper DNS functionality.

## Verification

Post-resolution testing confirmed correct DNS resolution and connectivity.

